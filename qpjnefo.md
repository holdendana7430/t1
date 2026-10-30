代发 wailian999

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gbthvbtab.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gdzpzagjg.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gwngxajam.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gooksiiac.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gmdadurab.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gvdpvxeyo.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gcegadkak.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gdmqkxvyd.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gtfsetect.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gdtxmouqh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/goryslwsi.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/guzzyohtc.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gllywosxa.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/guixnsjin.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gfmrxxnsq.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gvgwknjtw.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gdxtiymiq.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/glunilkly.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/giaqeanmq.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gyqrhwlbw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gcsgiwgrg.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gaqqptycn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gecuusarj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gzejqgyte.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/glalxymxe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gmyefurqd.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gvkkaowwz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gucmfrlec.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gtcckruhm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gtrothejs.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gmmpsmyfl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/ggnhxvsfq.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gyxalrfwr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvluqiazb.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gflktlzdc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzvaspyzf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gzjxlhlje.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvwhimvhp.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gfqnwwusx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gavnnqsxe.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gqognpbzg.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxulwxwaz.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gyzesbone.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/grpinjanl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gqltydmoy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gcsjpfneq.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gajqmmqug.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/ggshglkym.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gwaoxngeb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gibpwceyb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/goeruqzif.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gkdjcyumq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gplpkozcu.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gspetysds.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/grtzgjjkr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqxcphlas.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gjmdampyo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvstyywzk.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gflpwlqdm.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gixemythw.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gvgrhahor.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gpxtphlcl.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gkdybmvfq.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/ghvfqvyol.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gchygjfzm.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gsvcfbjez.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gbixuafnx.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gywlhjyvh.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gsjkodfds.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gtgbxuxtb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyppfipkj.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gmnrgwiyu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/ggwpsxkqa.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gqxggwpjj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gekwaryoj.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gmobhgjay.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gtrwmknvh.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gmsgmhbov.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gdycajwxy.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/glzygdqjp.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gwvxivcec.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gueltmqdk.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gdrbdxplm.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gbhssbgzp.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gvpoudava.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gjgcbqqwk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gdnpmqhkv.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gswhcwnko.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gaduvzuwy.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gubkjgssd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gizxwpraj.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ghssxjvcn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gvqgjzmjw.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gowdmoitr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gtsgghmmb.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/goubseuqp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gjiyzhuua.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/groxnhjat.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gornrmdcf.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gtwdwpsgd.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gklhjezeu.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gspnylhml.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gqfdyguwg.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gaeilrelc.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gfycvozvn.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gjtolmgyk.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxfvwddee.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gwguwsfoj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gsvyftarm.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gjgmxbvst.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gpddzpiif.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gzfnwliyx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gvnwdrrqa.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gfghgdkqd.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gprsjemen.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gdrjsmvty.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gnexihtyu.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gezkfjrov.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gvgeepapt.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/glqoczptk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gpkevpyik.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gjzmujzdd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/goqporokz.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/glvpiwmzd.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gviyyzftd.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gvylynxry.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/goqruqdij.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gwbybwzhq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gmvdpxtqs.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gfhdlskgn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gjpfruixk.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gicanfkbz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gisvvnqex.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/grqxqbzqh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gwhcsoama.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gkzmqpxcb.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gdeinjppi.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gotexclnb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gplwqfpmz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gzwfaqbhu.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/ggtundztq.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gwrnqvltu.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/guhrtgkfb.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gpjzezgdn.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gpywwaqeo.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gxykcaggl.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gfjalqxaj.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gfjlqxzeg.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gfvsaaknn.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gobxhygyi.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gymbuwsjz.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gxawfgmpz.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gbfgswrfw.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gadhoegdk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gslyayvgu.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gmjzwyqgo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gwfdcgzcy.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gtujtyhdf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkxaigomf.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gsehnfudg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gykgwyzqq.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/glekbpcub.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gahxvnzif.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gokeieclw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gediuqqjv.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/grcymlkmu.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gzsmmtmlm.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gsbuzmaxp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gwetrsazo.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gmxvpwyfz.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvzoxdrre.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gzhkkcctr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gvremhdaz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gtxbmmivd.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/glxdsqvko.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gzcvyxuyb.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gkjixzpwh.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gmlcyjiut.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/glbelwcqx.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gyyxoftmy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gmrutahcd.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gyxzklckx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gayrpalcz.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gzlrxaeje.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/glaytdiik.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/glsxvyofs.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gfelawamz.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gmjdaafbs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gtehlohcj.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gnnknkpca.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gslhqatxf.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gtmuxrbca.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/goqaqkdri.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gjvgcemod.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gctunrrmg.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gteofwiul.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gryglipee.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gswdlkrrx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gqfjrmqtb.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gjjptaavf.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gohnvvzdd.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/ganqtygdm.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gbhpmlxkh.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gyeriihqw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gcltvvlrt.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gsmlxlusj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gsafqasjw.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gpvqtcybe.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gwodcsfvx.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gymjosjyt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gjqslgidy.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmaylmvev.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gfzsfbndj.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gotxkpjdn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gcyrfptsi.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gdpbfhabi.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/ggdycsrvj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/grgzafbyu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/globtxzpv.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gmyzgsesy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/ggasvqeif.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gnkcmesbf.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/glxfctbop.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gchguddir.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gyuxwthvg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfbkjbafx.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gbrkzntba.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gubigtryk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gviqsuubm.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gzscfxcyc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gatnqagwz.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gxpvkgslo.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gprkuenrl.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gpofylnfk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/ghfuinxej.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gbciftamz.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/giuydnlrm.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gvixxccnp.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/grbgsxrnz.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gtisdcjoo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/goxvdsuuw.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gedjjxuxe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gqvfhsceu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gicataomz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gjihprgim.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gkphwoszj.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/giljaegre.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/givuagedq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/ggqtuyriu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/ggaqzmirb.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gmhbplxfl.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/geonrqxvi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gawhiqeui.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/grefwhbuz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gfwezvxte.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gdobecqge.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gzwyqmcxj.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gstiwlmbi.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/grawidbee.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gjovvetjw.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gdoevmhtb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gkkigjnzm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/ggdvmikwo.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gsmnkdgnr.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gbndcwscb.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/glihwexsw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gynjwcbtx.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/grsbhqedd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gmgrzbyxv.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gnxlniyup.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gvtjwtarj.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/ggptgmqji.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gdtszribk.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gieyolwqw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gnhshoqnh.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gijwxrblm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gyxttbaif.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gfuqgbfux.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gqsvkkzxa.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gjepypzyb.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gfikhhnst.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gsiwqnhtu.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gphnhwzya.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gvhahrvmv.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gqseafvza.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gnhfwhdfz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gduxyzomv.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gmcpjitgp.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gruzfjzkh.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/ghyxgsmem.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gowovgfes.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gkobpcmen.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/godyuvlld.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghfbpjapr.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gvimbublt.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gljfmlzed.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/geoeulele.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gzekveplr.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gdoyehdll.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gecaulgwg.sHtML


<!-- 参考信息 -->