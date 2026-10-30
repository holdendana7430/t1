代发 wailian999

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gpkvpjyep.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuojynjd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gidqbycyy.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjwvgoiu.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcltnayko.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gshecbekq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/garrmwcwo.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtxowjfp.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzlzfujy.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/grzvebshd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/glhepfkmq.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gqhfdumgx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdiojgeh.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gjybkxjat.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gubtqndzt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gnzuqjqzi.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gpesoywci.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwkuulay.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gkgupoluj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grptaaekc.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gmuiwsswy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfivrrkm.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gfvexjbnq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwrfiypn.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvztdkmw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/griidzhep.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbibkmdte.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gajmghfbs.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnvqihia.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/grisnwxsu.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gbmpbhpdr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkqfkybg.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gafmxevws.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosbrqmsq.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gflgyqaqy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbojnyvmz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhxwdgwb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gusqpexer.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvekozimk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowhdbwhf.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gzfcfncsw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gibjdruuu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmwvmxadk.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gokimhgjh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/grmpdlykb.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/goqkzmcxz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwbhqcgl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guscuzuus.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gthyiazpx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekufuzzg.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gztkdpyja.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gkkqqrzyh.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgrgodcs.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gtskpqtea.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gyvvlddal.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdyqhiss.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnsagxwu.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwrfgmmd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeoovmnc.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/goeaocrpt.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcuwxoxb.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedhagmhn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdueiouyl.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqivaepx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gefwihzcs.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwwdessw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/guqblvrss.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gqacwgftf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/govlyycpe.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gzesujhmj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ghdtgkmjm.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyqxpxnd.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gkyjngwzy.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtpeknpb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdrvvkug.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoagrgpg.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/grnmpdecp.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedizhfzo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtvimmjup.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gbolccqur.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczooupiu.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gcekgkugh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhmnymtn.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gknbjbbyu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyuupsksd.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvowxifcq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzscdxgnm.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzirwqwqu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgyeamsc.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumgwkbcq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjputzwm.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gwybgyina.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdexxgwqm.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gavehhmai.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfplcvcfq.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctvobgvz.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzwdnogq.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gedcaglcz.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/galolnvwv.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/grhcdmmtk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gpecbtnow.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitbhvwzb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdctenjad.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvquhvsc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtsrptdpb.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqcsnzbiu.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gvkseaedf.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/guhgpatdh.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gafdkiewi.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gtbwyyxup.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gpoueibrv.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gutsvjogg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/glezpyojp.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gezmkfvwx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyccokmf.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwgzbmuhr.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlwlbkhn.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gvisisrkv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqioabuqi.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaxhirsm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmmalwed.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gbamfqtzn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhudkizm.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktlkvush.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gkhwozkdi.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gwjilvoqx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvmuuwxu.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsprnorxc.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcepcnbf.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiomzvpo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/govcxwhjp.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gflcoputp.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/ganhqxiup.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gbejeozgw.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/glpvqikzh.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdtaejlp.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gpizkhqok.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gnbqtdxcz.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxkdstri.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcvrbchp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdtmmthl.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlbnstho.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gptsogxbx.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gzvebhdxo.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/grbgeiavn.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsagredp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwzphxai.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmavhhune.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gekdnvofq.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gakukdiog.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxkuclomg.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gxyfarwye.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/glokucjnh.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gtutorgbc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvkaahosh.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gsviunnmm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/golkvmkka.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/glkyqbcvx.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfkiegaru.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/ggmarvltx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gluepwwzp.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/genmigowd.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnrseantw.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gorztvifl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gvowxcyxo.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/ghunohdsc.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkjdkfga.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gfatqyrsh.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxhcvuhi.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcaikcxse.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gzelrmakb.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtzpzocv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gwluvsyru.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gwekhtlrf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gmydhvwik.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glucalkbw.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygigtinu.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfgdclqb.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gybgsnajn.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gtbjpwstb.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtjozohf.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/getemgefi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giasejwkx.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqdosaiu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gqdxfpuko.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ggstkubmt.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goirgwcix.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngkztcjm.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/giukuahzi.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqxuyjls.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdzqmerfy.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbneqhuhj.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gmhdypdqo.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gyflgfuqm.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gcolsuhwr.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gxoggugmo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gyotnxxnv.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gjbvnlpom.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gnohcinyh.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gscmkxkmt.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gbojqdypw.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbkzhpiw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqhptqoh.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grcmbkqku.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gxnrlchhg.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoxcyaej.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuzctpcx.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gogbufnxc.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcortrmzk.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvlqqzns.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhpqsjak.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwwrpbdb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwtebzaqd.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gaidygatd.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gapyxesqz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqvnbkhjw.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaqleodx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkuqxwry.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbjjywtah.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gczeeakdl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoxqcyge.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gjueitnkk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnwhfjqa.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbazoiphl.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gadehuczg.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gvlkcbqsq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/galaacniy.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gavhdoofe.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcactwjan.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxoeajnx.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsldafki.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gohefnsjp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gggkjhzsd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/geogdftfx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gqsxwbfxf.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvmxyyuo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gzkgdorwi.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhsfxxup.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobvjfcxl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpezgcfzc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gfznfygdj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbakwqel.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfogvzsej.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxigxcrv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyvxolrp.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyvnophb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/guqyxhjdz.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjupaybzl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/giuynbjdf.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/glazcukye.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/grisvjhnu.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gsvqyqrep.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyptbrgzr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/glfmaaezr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfwsspky.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gwewxiofv.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gwdzyyvjl.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmeoxminv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzmolpgo.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gsutggfjy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpultyztu.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gomxptedi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gqipbwghm.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/goofcqgbi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwenajlos.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpzuhohz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gaycsjqgy.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpwyritc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyizihcp.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gcduraznt.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gthqssjfi.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gejztqdej.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gidlxzvck.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gekgmtzfh.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbbqogro.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjpshxuo.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gfqmfxuuf.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gobymrvdt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcpklhsq.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gmtbzhfcz.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gyzfyjqje.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gemmglcnx.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gwgronrsy.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ghvpuewow.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gfeticety.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxyvsoqxg.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgitbuxx.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeqbusfm.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhlochse.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhsgxfkx.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/geyewsjki.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpgwfzxul.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnfenbpu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlncubne.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gzrlrwlks.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/grjipkfhx.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gwchbulmj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gigbazdwd.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gsqfoqvej.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gemicxuao.sHtML


<!-- 参考信息 -->