代发 wailian999

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gddqlgyep.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecjdrirc.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdkpiseu.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkvtlihu.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gpzpeydgv.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/goertbbyl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxppwzhoh.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gqspyksqr.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjharlpx.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsldskcv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/glaksdwpp.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gswepewzd.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/guwdetkhg.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gllusmvqj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/grwrzidlc.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhaxfjhc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywgwkcwc.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuccpobm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtwjbedm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gixukydvk.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/godbnnjvy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopzxhcqz.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxejtjviy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxekjanm.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyepymwdu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnjokatx.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnpuuphx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gpwsehocd.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpjahqfi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gesoocavq.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzckcsmom.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gaoghvywh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvsitwvr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcpgzcmud.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpuevzew.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gpaayvrcc.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gywqshbui.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gabqokeun.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gjbfbmrxr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdezvwbzf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvmtlqze.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawhcowkl.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzgefjgp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtubwbzi.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gvjbihusb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzoazadv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/geblbczfi.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvfzbaec.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gluyqzuol.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmrxhqto.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gazgokabk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghautdmqg.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxexsuhr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxeuivdp.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gadtofwzs.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcrvcrlk.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gmpftaaho.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/giaazjzvi.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gtyupghwc.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmmumfmht.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/goycwppxf.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/guxpoygrf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsirslct.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/ghclsjeaj.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtccmwesr.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/ghkhvcnwn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/goqvfnsfx.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxhiboowm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvljleda.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govioamhj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/grqypbzox.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gzdhfrxkv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gixnnxrec.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gmisoafan.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/girulkujd.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdtrbtbq.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/goexsijuk.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtguuszm.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gowltywdj.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkewzlkfk.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gdanviqck.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewvczrbr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfbvtray.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gectvoxsu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrmbawgm.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhvpcqrv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgrrpltr.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvnrnvdq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbgbyidam.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjdxfwqpo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsxnxwvt.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqunmzwq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwkkpvdhk.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gilxomgpe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/goownuucy.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmdneyngx.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/geeyreosr.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghthynysm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjitucydc.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjabupyw.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gazcvwxzh.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkszjdye.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gijvwoacr.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxoupibc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gucbiskej.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjfbyejy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwdmlcohi.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzxrhngw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/goqyqwgcm.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcyqjhsi.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gygcabzlw.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gohzopers.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxcdooau.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnwkolbs.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gwceywqis.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gksmfnifd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gspipgroa.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gdldcjvor.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grycudwmd.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggffhkwyz.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gswewfzuw.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiayqqgo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnqmkjxil.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gtdsqhfmo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gornnymqi.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzavumby.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gmtuuejhg.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gprdcjmth.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjmhtmrd.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqsdjtxt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusbscnsc.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gobmqovss.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcuasram.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gjtoleimx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gongtmkiw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gwylrnril.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwsfzyiq.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiwymfgc.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gbpzourkz.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsqduopf.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gbzggxcnt.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gyxppbwjr.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdtondcw.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gypjophsn.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gghmdqjxg.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gyhiklyxn.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gdifgammk.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpfzfrkd.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gfphajdvp.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntjuwcnk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gbqltvrqm.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlvwgaqr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/geqsnrkkx.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/guplyvzhs.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpxexqyqw.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giddbvsnp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfattlrk.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gynaiocvq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghrnrrabg.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gpetjlkvp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyiwlajy.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyphpcnb.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfrzxngoe.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpkdvppf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaxwoylj.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmagbrzch.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvoiuplmy.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gkqxslqlv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gcckihtgy.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gritikxed.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gtwpdskxy.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gypejwyii.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gkkxgszak.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gihwlyrrp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyljmkhg.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gaansuewv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/guesfhaqt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppazaaem.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gbdwhuafw.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhfevvvt.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gedcmlily.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grvxamnxd.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gkzhjkrcf.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorqgdykh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzqetege.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gplkhtfyk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctmkhorg.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gekjvzpjd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gprymlnua.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gjmjxbmgz.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gpidlfugs.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/ghnkwcuja.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdbmdnff.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gmyworrda.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwhtyyrgq.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/girqgnlme.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gmhmibjgi.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gaemwpfwa.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/godjewpuw.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gscoftadv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzaaohco.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gtzwmgcga.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqmeeoxg.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gszqyeydv.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicfiykws.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/grwjekpan.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gydlytsmd.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxxwvpwjh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnrbdqxh.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glpkoxvgd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gnivtaaxc.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gxethkesv.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gflqdbhil.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/ghforqcra.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/guragbiot.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzrqzfjb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqcgzeta.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gfvczjuhh.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyggplyw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmifhscb.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkslxjso.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbykgqetg.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwanvvqmj.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeuazxzk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbapkucsg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/ghotjtzmx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtwjlmjv.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gwzdcgoyt.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzyyngwv.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gvqpaccfe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjowbysp.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gskdlsoit.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gjjadjeed.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/giigffrrn.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdtgtevq.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gdxoqyagl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gwjnlpunc.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gjstzdhqb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/ghdwbmhxy.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gzutsziiq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzyjtdjk.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjdevlnp.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/grlrpgavy.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfocztivf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzihrbmj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/guuqypcxm.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gxtxrvpqj.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhxborjm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbehnmtr.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gophomndx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gddmiikwg.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gbevijkmd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gceocczcq.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gfnfaogvv.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtwnlqrb.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxdcuvao.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsepaydjz.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopympihm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gdtgwzckx.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnzenqfy.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gedawawee.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/ggsndcbeg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbjxnfli.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtpcuksi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjunvuoxl.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gzagykxhl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gauhfdlbj.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurlrxhaq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtexuxnc.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfgashix.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnwirhdl.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeqztied.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gkvdbblmp.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjynjqeq.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwecllesk.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafursnbw.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcghpdzvf.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/geclqbcbv.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaoydvxv.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gfrsugumv.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbdjswkk.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdxfxjmf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuwcuiom.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gncgvltpv.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gldkjyiqz.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuxmqpoy.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuandehk.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjermkrzs.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gicrmwodd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfhiopqec.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyixktmzi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnvszjua.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/grekphzjy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpilhvgil.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekhadkld.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqdenffa.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gusvqaacn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gvpjhnepw.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpueoevhw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gumaawqww.sHtML


<!-- 参考信息 -->