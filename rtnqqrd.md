代发 wailian999

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtbaqupo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxbtlngg.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gbmsrcobc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/goejbrukb.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gnqxzeoqa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/glhufgpdt.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/ggawbwagn.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gdgmwmnbq.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlgzzzpf.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvqeecvx.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/ghtxvlntn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gbsfzugjm.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gobzhwvqk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gtxsdevbc.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxtifglk.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdofgkuzz.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnixtlecn.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhnnadol.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gqqxjtpgy.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gorolzokx.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbuyqvbx.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gszsitkpz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gnfjtgykq.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/glunjeavq.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gngkvctsq.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gindqtwus.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/guscmwhxd.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfdjonab.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/grdomcmpc.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gvuoqduqg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwdbmrmj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gsaapoxxz.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/grqqevhyw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gosdxazow.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtkxvfpf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gcncpzamn.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/goxveagbd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucwftbcy.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzjabdgi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/guxgtavun.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmnrbazc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqabulba.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgezuhsv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrxffacm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkwwguro.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfidttvmm.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqsrrdew.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfejlkdyn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgqjgpah.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfrafwzsa.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdzwbbzu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfrflens.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gajfjcmpr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gujvlvijj.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gezcjfomi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gresodjpy.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/grwhqibjl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gedvwkekp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbvloepkq.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gznkmfash.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhxkyobg.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gkudphrps.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyevzmyt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzsfyobgm.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gweynonzu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbeiujfym.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogbsgkxu.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvicxxbf.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhnjlcih.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gizhhumxv.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzthzvof.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwzygwnkv.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhfkcpxu.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjwdcyzt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gronjvthl.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfzhsifh.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grizhtdpf.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gcztqhvba.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gltibjqsd.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmahnbpk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gbzwawrli.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ggifmarna.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gyoodfync.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/geumutovz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gtxakvemi.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gdthxpbax.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwkjqjah.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gecrbeqds.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gessgmcnq.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbwznqgx.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbtwjpbk.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsralnxzk.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gxlrothwc.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfzlbrgwl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhoohbmy.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/glkuabaab.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gacgekqkp.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gymnjsfpx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggimktonc.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnizgpaqi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gencciugw.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gzggoyjaf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gifdpqrjg.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gykriyvuk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gmdcuhbqx.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gcsvtwizt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghczjhdvg.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrwddufw.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmrtwkiwl.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/ggwlcbuul.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwsdioyyd.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/galccnksa.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcdbzqced.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfzxabsz.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpffjlxqz.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gubkacgip.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gihkjkxpn.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbojzbwq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gchiobfta.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gtzlaotpa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjjvvorto.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiaavfgh.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gbwwyvsxc.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqgfozcl.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gptrqdedo.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gpyledkis.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdjwuynu.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpoqnvuy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/glgnpyzzm.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbeimnue.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/giallpelx.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyvbkkgp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gswyhpked.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/glcjzmrde.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwvebhnrg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxwpintr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpygoskpo.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/geezliuns.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrdzpioz.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfvxdxsg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/getbuiniz.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gtczsfkrf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gjogdoxuc.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/guphgymgk.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbgtofne.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnlgkzao.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gjllehhgm.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/giowaviua.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/giaylqqdf.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuodapwo.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gbuidtgzc.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/ghyqkdbrc.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnngithx.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgwkisze.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzbtxywjo.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glocfpfac.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwaxdfzq.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gzovwqyyc.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gbougtlpm.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbwqcico.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyeqqmsy.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gqdzxshqp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gkryqsmru.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grcwsibvo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzvztwrmi.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gryyordwo.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gybgxlhty.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxkogrwe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gomeerbtn.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgdypsum.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gctjqybbx.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmmnxnvb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrlrxgcl.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gqqltimtg.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaeqcffe.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gjmayqvrl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gytjuqirt.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/goxxlowsh.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxtbytofp.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxxhdggg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gnmlrqles.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gxajnvryn.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcpwepqm.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gcrmvyerx.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqqmzuxs.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzaiqhrab.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfwdptiu.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiglpqgp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/grccwnpet.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/geymcbwqm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzjwkzna.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbaanquf.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/goneygkzk.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfcveyec.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gvresbsvs.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gwakfdcyi.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gtphdvriy.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gjksqxnlf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gcvuucwuq.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/glrqocohb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesdnnfby.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gyvwvuzrg.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobnaybyj.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gsygygarv.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gylkckpwr.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcismpfd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmzrkhmpv.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwsiuavj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkphbzdmk.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gpepyvmpd.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gszhnhwss.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gszxpaegg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkuubpjr.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvdlffcy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gntrzcqsj.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gqtabtfqg.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gqosbogjc.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdwjbopr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghkaupxm.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitcabhcy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/ggzxxnkrd.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gscskljqu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsgfsmei.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gepyxteas.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmihwbuau.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnrhucmj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthjuhgus.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gqnqludqb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyrmwkuvw.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrstoieb.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbxxvint.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggubjekjj.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnqktecq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkocuchfl.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwomzykvk.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwtbnxnl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvzdwfco.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/glqdfywaa.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsgkehpl.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmckgkvds.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gihphkseb.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/grwdnuyxd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbwbjygk.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gicjfjesq.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjzthmumf.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiiqephd.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gokzwjzfp.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/giztkiqmo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/ghqtrsfrs.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gkprylzqg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gpmlfoeya.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gracaqbwt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gcgiffgew.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceyvkxpx.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gacmfulcv.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/glzdarmnp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrvanvtf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwvwdmsp.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gszzfqhlz.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptoqtohn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/globbiiko.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gtptlfqiq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gwwclzvpk.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhpwwija.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/geymsjjal.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpatnbhgq.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/grwpdwxmi.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkftpknib.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfqwbgem.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gujfzmwyx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzbuagwp.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gucuwoque.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/galzcyuch.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gsloinnjx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmzzqrck.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoiasbjf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtchtraa.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/glnffygul.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gmdbnptjc.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcuddqva.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gzkcdptzk.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmagoxox.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqatyraa.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/goadvyhce.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gcoaczxqk.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gehsknszz.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjegqfrke.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgdynlsb.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gaiosukpe.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrgxvzin.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbebbqkk.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/glqmwffmb.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwadysvqv.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyrrvrnfv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gazwygple.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowmnoeag.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gwajptqpi.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gfnhmkbqv.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gwharmevo.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzcujhkdi.sHtML


<!-- 参考信息 -->