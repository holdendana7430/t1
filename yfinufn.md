代发 wailian999

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gnurmjtxr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gexnrhonv.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gucntfhbb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gamjobwhg.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gbqpvdapd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/glbbjzvus.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gpougkaiz.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuyojpfk.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gsfcqpkwq.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqqhxaey.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdbitqmf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmfycivq.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gcinzdydx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdfibbdd.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gfbrireos.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwizmhcpi.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gpyeylslg.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gqgtjlyvb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gusnulzei.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/glfgpblxh.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggrigookd.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpgrxizc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/glleiubqr.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gaxleluhl.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gueekprcn.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjyflxyg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gbgzvcuxy.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gvntikzqb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gfvvtgpkp.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gwiapfnhm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvrkscpi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girscgooy.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhehderl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gpoywxall.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gprhyilyz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gyuacfxbv.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gtaxjhxxd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukeaynzt.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gvzsacolk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqdzjgnk.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gxjrtbeku.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gziihbhnv.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyunmfje.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhikxtsq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldcdfnbn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdtshzuqh.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzngcekd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuczkktz.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/getdpnwpl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghldskvuo.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gpqyxtibe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gcczabowe.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/guziapgdt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/ghbbyimet.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvepzwtlo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gohmvsrzd.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gooczcicv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gybmcwpql.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdfoxpci.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gillsgeat.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedynqnvq.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gvhimaawn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisybazkd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbilcqjgn.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdtughhb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/germjyhrj.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gbvkrusut.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gsivpcjul.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gljsjcamy.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoibzzob.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrwrncdt.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjmlewag.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/grofdwsux.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gblyvsxvl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gjkzozpga.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpoktaviv.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwsjxniiv.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggegvibe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpmkrzhxz.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gebzdljgf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gaasmpurj.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadtthscu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/geqtfvdfl.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gkihokakp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkybjmqi.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhxfkbvi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ghvldxjbf.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrsumnll.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gcygmhweo.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnrsjfso.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gxehtbqzv.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gpdtyhnza.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/glaziaiza.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grzxitxtw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjoqnolw.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmpknekl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlqahibo.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmjzudxv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgzsueyt.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlusekck.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbloxtmi.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gyjinucve.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grxnnupdl.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqouzizxp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gilcxkbep.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gxccwsutf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbytkpgdr.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwvvunpv.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwciovdgk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaemyshz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqotecti.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrqivqrd.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkkqeesxs.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gxdjdxqjp.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gixznofjz.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjmbgdzf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwmbogybz.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/glypofkeq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjreeldog.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gnghxsren.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzjyvxux.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/glzkpxfzx.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gkascnrre.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwlnknqa.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gtxffxnbq.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcnbtkum.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymiuxdse.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcqarhuqm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyikztyq.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gosdhkmmo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtcspiar.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdudrewo.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxzkjonkj.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhruzakq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkbzurtc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdxhoend.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gevpjfddg.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gaotestfk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgjlbhsf.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbucwisb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gimijykog.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegdmqvfv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gbblwuqhg.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcxfyrdlt.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtwqmlxd.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpnltapf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gdjrkidjv.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gdkqskbrj.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gpznlyggd.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gipbrvjfo.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gwcimotby.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gxczcaxpw.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkprddck.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gumemotmp.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gshchtcpo.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdeksfpx.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gneplohfm.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjurgacxh.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwtiqycjw.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocxxlqgw.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gypvoxdtu.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/guawhbcjv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixuiooon.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gaaasfdgm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtqkonqz.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/grgiqsvwp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiasuymh.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gbwymhkhb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjucsuiy.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoaamusp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ginwgmjzu.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gsnvexlve.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gavlicwiy.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuedjgvj.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glptebkam.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjzyqizo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgcutjep.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gytortaag.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gubcpuicj.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gcmcsuipy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/ghtmwaape.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxamisnf.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlkxlmkm.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/ggtmaxwpp.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gaojlxdpk.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gznyfoelb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtsyejrd.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqcrurlb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxthywikc.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrabyzeb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gulqveubb.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqrmenvv.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gcxyfyamp.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvrhvkbk.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gktsgxuhh.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdtjmlcr.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/graljwvtu.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gdlzqpoqq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdrejylw.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnxdvgso.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrtecbin.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gwmkpugsg.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gprdefoum.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/guzbuulhz.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslhlsimi.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyalqvfk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojpawvcp.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqjfmugt.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlmrwtda.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gbyhsjyxi.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gzmmaoakp.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzzxvwacw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqidfpkzj.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqkjaeli.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvtswtxka.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/grujwxulp.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gdtfstdle.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/grhgjnckz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwssugdn.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqowrxrhm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzejwbwsd.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdstaems.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gyndoxcky.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gveahkfhw.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gdwiwdgub.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gchdivxtu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gesxfwiuz.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gedsocgqf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggtuubwbp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/goolhcfga.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfrkoouy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuhtpsto.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaevuiyh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpwweyyup.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gooscpiyt.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gxfgfohrd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gldegfeep.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvdeafjp.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gghufeivx.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/geiuygbmw.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhtugmsk.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/golojjddd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpngxuks.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gseazcugm.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjrwozrt.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbgsnasv.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gjujhrtst.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhxxasig.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnscwiie.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqowdwoe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gmyoamcuz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpduwqih.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gauztsplk.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gjhcgvbtj.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpetobpq.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gokwhigxl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gdzxqvmbv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gwrqvthwf.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gpwlsyqby.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkeezbvt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gkgyelpmh.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixzzzaew.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gdcrnsbyh.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/ghriidisx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gluvpntyn.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqluykmls.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gpmjysqmh.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaaiqdyi.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/giwhiegay.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gllwbtgiq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwgsjkmy.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/ghxdzrmcp.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gtpzcxwqy.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gicgrmdwf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfbvwfgt.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlxavcyh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteyeyezw.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gzocmrsco.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvprmbkbu.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/glzvpyulk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwxoienn.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gjtbvqvsj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmihvxcw.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gljxiervi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gywwhdtyp.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gfynsmluk.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpziuflw.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcguyecvs.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqsyanxc.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrnedfgp.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gtabgdlci.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmmbumah.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupbgzkyh.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/grhpdxugo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwvwdiek.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gjkiamxql.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuwujjul.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfmcyqjf.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjevghwp.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gclpqcjkw.sHtML


<!-- 参考信息 -->