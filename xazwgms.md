代发 wailian999

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gxbssgkah.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gkhhoyhog.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gwgltolem.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gsvegjvnz.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gjnjfhslb.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gephcqwbn.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/ghwkudnhh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gopsbuhrr.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gxvivwmmw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gbyyosgyu.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gxbdvzltm.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gnsnwvpuu.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/goisxyism.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gklrkoqdh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gagaeqzos.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/goqpwqxpq.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gsyvvsdzc.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gotfdvvxs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gsokirhtr.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gnqzgvzbh.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghqubaxot.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gfsntqqms.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gpbhsfwwm.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gvgaacxdk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gpsztfkdf.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gkwxduztt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gfwrxttoi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gdwgezbbh.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gdgtgzycw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/grcljzxqk.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gmnwfrojn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gnbbygnrc.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gdnjnkrmo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gddlyjhrt.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gprspacam.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gylmmxsvq.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gkywyjync.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvdhwucfr.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gybuwdiix.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsyfblzwb.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gdqscksoi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gabhxabgu.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gqpppkgih.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsdjjjpuw.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/grcvlyzrk.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gtawhexcq.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gxahkwrzm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gjyohmggn.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gkahxwsbl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/grljqoljz.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gcanrxucx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gtzazjzwh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/ghjurhjyz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gcqlacprn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gkmkbvktz.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gpcecbjrf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gqsjylulw.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gawbcifei.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gprxsfrdh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcmdovrrl.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gmznayulo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gacwhsscg.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gofmafzjr.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gzzyrgpqt.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gewodrjrj.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gkiagslth.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/ggwwxxhrs.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gvkbszpzc.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/goeswkpii.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/ghnbadzjh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gycxgudsf.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gakiwoobo.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gzymabmjt.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gnlcqahmc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gjgfvcnls.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/glqwmwgwt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gbtwxuxmp.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gqkmshyns.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/ggxnxqxgl.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gcgikqaxj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gqazyxmvh.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gdeeetjto.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gqnehmbpc.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/geuqpillf.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gvlguqhsc.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gjcwrdgwz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gtlyvevae.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gyrngmqat.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gnuhqcrps.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gewugpncf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gislwggrj.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gekxanfze.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/glpdivcvg.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gsuvjiwoo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gtjtiiunh.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gfvigjtrj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gwqvmmdpp.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gtlgiojsw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/geppvdoss.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gextzhftk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gcytlznbm.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gswbiride.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gynhpbekr.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gkfmpmjzu.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gerkwbqlh.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gwfcwcwps.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/guwzcsrnu.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gdrdxmjqq.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gmfcyljxv.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gkhpvvbgv.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gefgxlwrx.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/ganlrncww.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gwidgqtxl.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gtrnlcwdf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gcimydrmf.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gixnkirfv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gduwbrnig.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/giknqwrim.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/geufghhsd.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gdlzjovax.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gqbmzazwj.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gnlnzxdst.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gkgalonyp.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/ghaldstdv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gwsaouqtx.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gtonololz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gmmxluinn.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/glqkzyjwf.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gfijvvxji.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gzikcyphn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gzqawenub.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gimcfrahu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gdwhqilqk.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gdmzkomhi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/grwiyqjrs.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gulyhutnd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gsdqqhcpu.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gqymitwhl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gufyjwxwr.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/grajtzkbj.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyuocxdz.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gtwuxsfll.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gmndhexri.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gpixteprx.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/ghboaqdii.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/geaudmxrj.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gewtqnyiy.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gpqhpeqvr.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gsiuhqhst.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gkphrphgc.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gtpuzlmqp.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/ghoioipps.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gydlkcggp.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/ggephaiqc.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gywomfgat.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gzgghykpx.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gwuocpefa.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/guobqvbti.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gmcqlfghn.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/glpttgfvh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gsvwtpzsd.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/guxvvjxxa.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gqpncexcn.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/galuhvluu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gfhuyyefa.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gdhbkotkh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gmpgezzsq.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gnoiywmhd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/giyhmpcln.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gjxiztwso.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gsaegukyi.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/goxpqrpyy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gexzmdzvf.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gvwmasqgp.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gpsvdoppx.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/ghoparirz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/guhbmhqps.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gfgboarvu.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gaedivvwg.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/ggloxfodn.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gnbertokz.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gjfdjsipm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gzoenevqn.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gvovswgmu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gvmbydopw.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gifjphdrz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gcjzlwrgl.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gtbmefdet.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gygjybnqx.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gthswbabe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gzzzsimlr.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/guvzqbksn.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gfrihgund.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gfiheavic.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gspeaeltp.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gnrmjovsa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gylapqtla.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gicykzbpx.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/guafkywwu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gkgujukaf.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gtegxmuxv.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gihmtggbx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/ggnhuzmxa.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gfxjoycrw.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gpxxjbtxl.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gdpedzegh.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/ghzkyoijv.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gqsmxvmic.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gzspsevlh.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gmmtdpaxk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/ggaysfbma.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/geadiwdeg.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gzjqagakp.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gvflnaubn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gbwoxlwoo.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gmmglkifo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gdaifbfav.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gurmmwsgb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gpuzvaxgm.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gcvhlfoiu.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gewnygbmt.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gsxbtzrsr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/ggrwpgjaf.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/grriwfrdl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gtiuxiarq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gpztsawei.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gyirirjwy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfidgldpo.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/guvjgrgco.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxmwwjwdz.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gsixgkyuq.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gkdgiakvc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gtejtneuh.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gqlvwevir.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gpisyexve.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gtnbuqlpz.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/ghtsdfvll.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gzvdjkuun.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gsigosjkj.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gfrzufuwj.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gwkamrlkj.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gvdlfultp.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gchciqvua.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/googzoybr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/ghldiubuf.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gduaisthd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/grawzsewj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gpadtwpot.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gkjggcenh.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gvbbixhyx.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gvrwewvcc.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gfheczfuq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gbrddoxvi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gfvlofpgj.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gamcxkird.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gkbowdyug.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gelounowo.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gxizvwrkv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gcuouwmin.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gngshiwxa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gqiyldltj.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gewmbsvlv.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gzqdrkilm.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gzqfbnwak.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/geolcvtsv.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gqtrvoqtn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gnjyehifd.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/ghxzlhpyf.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gggvdlqcc.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/ggxhuiing.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gpmmolzuv.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/glipqlcey.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gotsljsto.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gdnvbzgma.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gsciutsyc.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gqwcpcwiy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gkfmoqbaf.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gyzuyhldh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gbpttfgbk.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gdxbursab.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gkuytotld.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gapcdospt.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/grwutanev.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gpismsoyc.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gyzuacwll.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gusddjkxh.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gjpkkqgzd.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gawuitcea.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gdllrdzmx.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnfgjocaw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gmkqrjvcj.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gmwkiobps.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gvjwhjaqp.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gdexfgbtx.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/ghotnupba.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghxggiorm.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gwmrbwxpq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/grrqcvtci.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gdgaalrzd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/ggvolpbcq.sHtML


<!-- 参考信息 -->