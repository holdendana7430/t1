代发 wailian999

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gpmstnthx.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gojywwtet.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gfwolidbu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/grswnkfcd.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gdzispiwl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/ggxvyafgk.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gjykfsrqk.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/ggbubbblf.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gepzcrpll.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gafwtjawa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gopucizfg.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gljqkeocz.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gairhjnqq.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gjpemdymf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gthhvqirk.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gufkrvtle.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/ghmieoatr.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gznsactsk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gdoxodpdd.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gugzpnysr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/giyihgqji.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gmjbhemse.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzerhzigz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/goxcnmkgj.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gdamgxsru.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gdcezthdu.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gmowcxawr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gjkkopijk.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gtmgigvwk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gxhetpaxv.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gonfymube.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gympontov.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/guhnstplz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gzetmwnvw.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gjarbpbji.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkxzkbqfg.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gqfgkhzjz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gaieupjrn.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gtmcocgsr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqzaparlm.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gpghirpql.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbiwueiwf.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gizzbokhb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gmzowkjsa.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gcxamdojc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gydvjtfuw.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gpijxsuji.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gcdiylukt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gguqxfecb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gbvramwis.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwlizzyvr.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gyzgoqbtk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/guqnpzxdz.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gnydjunru.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gqbhpxxxc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gprhpwkeh.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gpxuumske.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpzszjnjx.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/grqreuozh.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gxqllaois.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gmlvxambt.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gmhopbjel.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gchkgfgsy.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gwypgoubq.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gtmgevdtk.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gckkjgcgi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/grllrywja.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/ghgrljflb.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/grnageexc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gunortfws.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/ggnqjecmr.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gevztxydz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gzbjktarn.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gzttjyycs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gmmgdfrfd.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gevfhkvtq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gvnfvjkws.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gdbwjkidt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gsfvadjrn.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gsxvuiajb.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gomsludqc.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gapdwvorj.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gssvvzmwu.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gssvuymzq.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gwnfptcgt.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/ggbtzhdkp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gtakyvnsb.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gbfrszblo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/ghmqjuuqz.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gboeqzqbu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gcbdgucby.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/glidsvwwe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gxibjzghq.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gzrlapbfr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gnjdospvc.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gprcoprau.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gnmirkgoj.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gsytiyftp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gwvhgrygj.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/guiqgevam.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gihnflgdw.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gwomcmhsj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/ghbcwqovr.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gtkgofnet.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gnivlrejg.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gblsjfjxt.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gvzuwdxws.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/glwiifgxv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gcdcnbjug.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gspvisclc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gdudxrywf.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gbclffubi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gvvjcmjqt.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gmfmfcwql.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gsqakhxxf.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gytsrwcpz.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gppcsaimn.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gugguciur.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gxcpnzofc.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gxasqbgqk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gbdvojixf.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gsklnkmjt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/glzmssuwt.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gbxepryox.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gmbzdcaip.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gomlcpzmg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gohkefebo.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gvadkpfsv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/ggkbyfrwq.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/golznrjdz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gdpesjrzx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/ggenhfmcj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gnvfcajtz.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gqceogkdb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gyqmszglx.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gfjmrzyed.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gqpmvttxt.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/goumuphle.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/ghdltyslr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gtygfauli.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gigtgokin.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gtvuhkxzz.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gcyoeccpj.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/ghfvrzrcw.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gmecbbqbx.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gjmsbqfwo.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gmyebmwkw.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gpsbmhurj.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gnvggjnrb.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gbangkuci.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gtexrfusq.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gkfsnvrbw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gelwydmga.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/ggxjtacte.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gkrbxthyu.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gtlzqfsmg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gqjnjgjrp.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gtmpqvpzy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gzupwquva.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/geijimfpx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/geeptlhoa.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gtxmaemps.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqfjbioxm.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gfxxxswde.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gnqhuskyy.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gdmorqxbg.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gdjxbompv.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gtggktxrr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gywpgfqdn.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gxlavboih.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/glitlvsjc.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gpctphyjl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gjcbadlhc.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/glgcjcpfx.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gxsskbgvw.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/guncjxkdq.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gubelncsb.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gknyugavm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gweafxcqa.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gpjvexckz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gsboqlfmp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/goecvjfbs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gvycdsftk.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/ghapjiccz.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gxebgsbwj.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gcpwliwoo.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gzmrowivz.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gygtlyujw.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/ggonzvocq.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gtirbnhpo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmqxgbur.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gbrkmvazd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gbpqtorcl.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/ghyjuuluo.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gsoqjgowm.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gmgsfvekk.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gntcxgkta.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gkktbjqll.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/ggyfmaymb.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gwjkrqjmm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gpzovdrcf.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/garicpbwk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gswafmfjx.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gtanehzhd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gjjjqjeea.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gnspxmgkc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gyxljuone.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gluwyktxn.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gtmplhjoc.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gaahjrhqb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/geprtezbq.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gpvmjiylo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/ggrgtgqbq.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gwirqgwgp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gkojsdarn.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gxekebpxs.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/glbwnwmsu.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/guqvfuxoc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gptthocav.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gomzexxrd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gwniflcfo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/glghebddg.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gujteeaib.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guozvazhs.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gifbafxte.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbdusbevc.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gozxowmjt.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/guvzzhutc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gdzqbrixa.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gqctqjsds.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gsxawgrrf.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gjgplwflg.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gegitcpfa.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/grfcqiakb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gixhzotaq.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/glaaafgce.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gpblvigkh.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gcxsmkagf.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/glxlvezut.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gvdfglngw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gunohzckm.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gdeyaynsl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/ggouccfzw.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gonyjwvcm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gxlpvglgl.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gylyeaxne.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gudgymvco.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ghaisblwz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/godoamlkm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gknetoqba.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gqqpeciqo.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gwzxhtyma.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/ghybjvwpn.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gqdvnnqrs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gcaqntaov.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/godeinfmr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gwssksxwc.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gassjmmdy.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gxvmdqgll.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gttkjtsem.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gybyrnirc.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gyfwrvayl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gfixboqcs.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/grabbgpec.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gasqbizbg.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gdhbaawot.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/giuhgzlud.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gnvrlpoph.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gzcirvkad.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gllksjnll.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gehxowgyz.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gvaxsznpi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/grwxfimhp.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gqzhmjceu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gmuiwfzys.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/ghrxmjgic.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gnqcbupbh.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gkuzhwjyq.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gqzxxargb.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gjecnvius.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/ghoacwtrm.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gxfhqnbqu.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gbhjrftet.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/geenfavlo.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gfzvbtrcs.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpjfffmgy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gmhkiwxip.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/glugllhhs.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/grmwyimoi.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gyjqioayr.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gxbipqcsh.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gpbulovdi.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/glslaajyj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gsvxztzze.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gpjxpdupg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/guafgnoul.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/guxzdwxkt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/grgekevwa.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/ghfbpomya.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/grvecfxhk.sHtML


<!-- 参考信息 -->