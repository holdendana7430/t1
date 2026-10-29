代发 wailian999

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gpraqvibx.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/ghkmukdqc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gzppnvcch.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/ggdetlocm.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/ggcoalorb.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gihiejfpg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gnuokiuqp.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gwegrbbug.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvxhzdbvv.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gdmofxhkj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gnvdibgxt.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gyeyjsmjn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/guenuksij.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gpoxibjub.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gwjftzdyb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gemxsdefv.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/grrjaplbu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gzpfjtfmy.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gevpipqds.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gcrmzlyas.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gvbocpydg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gfoxssawl.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gmenzepqn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gpjcgxlsz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gazzwvlpi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/giffzxoqv.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gkhxiqwjf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjguegeoa.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gqoxxwego.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjrjpdtlb.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gtkuwrqpu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqioxdpvd.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gqprdryla.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gleeidlkr.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gaceunzjs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gfmasurhv.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gucgvnjsl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gwyiqryhj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gwswribfz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gynwygrwl.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gpgugcrgb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gsumogzlf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gusnczxlo.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/glhlcjxjr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gtwemhxhk.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gzajkznhj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gzosoyhqr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmpjvzxzj.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gbhlykbpp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaujamtya.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gjlbjhsvn.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gneclhswf.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gfrxgsrrq.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gessabwke.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gcvntcagl.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gjwlsakil.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gjamjrqtr.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gpjrfaizi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gihzwnpbc.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/ggdmefdnj.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gwegykxgr.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/goklfadwf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gvevtwssp.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/geqsircxi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gqjjgnwjg.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gqcbekaro.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gdelnvdtp.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gzvigajvm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gsftszgky.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gwpgsrnwc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/grmsitszj.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gvjoemamt.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gjooctszb.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gyslhqigp.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gspcbrowt.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gzqadlavr.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gcjemgbow.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gypfdbkvw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gqhvwabgy.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gilghjqev.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gzwgkfhqp.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gcwcfcvfk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gwijkychj.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gaevdvrlm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gekqwyzus.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gqcwxuedw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/ggvppsbdi.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/ggcqiopxw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gyheuuvzi.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gcjqbnnwa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/ghlreowvx.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gkertgslf.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/grvplqkvk.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gmpltbdlh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gaetjthvv.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gkghiekal.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gihflboza.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gdnbdvknz.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/ggixsultx.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gtqatcynh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/giqbthuxv.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gvaugyanc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gowvwtlqb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/grmeckckx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gcanlfyvh.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/ghsvubvmy.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gepidqgev.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gciubscmf.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gzstzdlkm.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gnnxqxuic.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gmcdkeqst.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gwyyyjgxq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gwefpczhj.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gcbeoapbv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gvhqluihw.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/goqxrnise.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gbdmmwpye.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gvnkwcwfg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gtxrxjtsk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gacsqzhpi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gwexsvbos.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/ggdidajnz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gcuxwzjrh.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gcdvonuiv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gzwetcjth.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gtxhxrvjh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gcaujpzjb.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gvymzsejs.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gtsixrgpb.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gyqtfhrbs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/goycbydnj.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/ghgbaqyxe.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gfyyswvbb.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gccwpxpdo.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/ggvbxpyio.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gyjjcbmzl.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gqaingkse.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/glbnbsucr.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gfilwzsxa.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gjylmaznl.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/ghinrbvyv.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gsenqadjj.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gfgoipyaz.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gtixaefly.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gtigzoibm.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gtbhsjhpy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gzrbpojnb.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gpoesbbbs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/geveogrjg.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/garmlhrbr.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gablaqsly.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gceswfrlu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gfeotjlay.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gcqyzkmra.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gfkvbuwix.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gcjtblbbi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gubegtycx.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/ggvifnjaq.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gumuuscgj.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gfdvrdiqg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gkcukupiz.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gnrmaleus.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/ggyifhnbo.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/glqzqwjgt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/ghuizcmix.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gnnyhjyfb.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gtambgnax.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gagefkptp.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gxwsdnkjo.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/giomdjzew.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gdjhrkkco.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/grnrwbxfq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gmxmseuoc.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gtcjndpbr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gklvsthdx.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gemnngrmu.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gkzhrypic.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gtjkeextv.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/geosiztro.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gtwpwagdy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gpcgniepm.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gvbawcubw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gxvgfkvzr.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gzhebrykl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/garyevmjg.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gyewzazpk.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gaojfefdp.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gyowmvvjv.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gwtkzcmcf.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gnrfwvbbd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gcvmcagbl.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gvgzajgfg.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gynqfgqcu.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gawgaspjv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/ghhspcpgc.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gdhubixnk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gipsfeebr.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gmvyhvebx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gmayuhnwz.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gnfvxzvhg.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gekjkihdr.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/ggnmhuict.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gmoaqhtbd.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/goolytxfx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gfedpwfyy.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gcpmhdaut.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/ggunhensa.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gsyqximde.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gqwttzwhr.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gnyoxldok.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/ggdrbuhfe.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/goawtkuas.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gqrbcjkom.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/glvtnuzpg.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gbstwfoxk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grczgdbwh.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gafyzjrbo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnueewijx.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gxkmejeoa.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gldplkfcn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gpeyzvqkx.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gbfwcnwdh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gkkkvqorr.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/guducjofb.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gvtelahyz.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gblclvfzw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gbmkstzzf.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gxjrqhnct.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gkleainqi.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/giahdfetg.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gkegwwkyh.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gsyicqmzw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gkmovzqoy.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/ghcuuaggv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gipeffxae.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gijxpfjjj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/ggiakljzj.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gcwhcjrxj.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gqxmkmmym.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gswmgknrg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/glkctnbbh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gpuxrbfeb.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gcsdvdbtf.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/grqhfqfcr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gavullkab.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/grmyvkfrk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/giiuiclpd.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gcvzegygk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/grhrcsupu.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gmoxjtglr.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/ghyajcqwl.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gmiioctvi.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/giquwrsps.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnuzwhnkf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gxkdgbfqa.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gsheypcaj.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gznzcaxyt.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gbixcdagg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gwlzcqhez.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gdykolehq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/glpsuoetx.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gckrmznui.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gvusirznt.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gqhdvzfnp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gbvfxikie.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gwcfjndhz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gxdrzzoad.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/ggkaxuxws.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gdpitonpq.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gofvjonvx.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/ghwlfmgyd.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gdhjuorrl.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/grsokjbyl.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gjfvgmxvs.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ggdekjbas.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gtljwhvvl.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gftkyrzgr.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/grpmvrzwe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gxymrfehe.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gasptbvor.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gdfdvfqce.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gjpptzudp.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/ghcteqphx.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gbslrazks.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gvjcgppvp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsbdhbudd.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/grhkudkup.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gqbftzpto.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/glzbttqia.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gkjrdlvjn.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gmzrlezjs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gapcxsyag.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/garyfqnmu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gnnoitlve.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gfeuykjzm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gqolxzpsw.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gqmyqrjkr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/geoydmoxh.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gimgfgmte.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gdtcnsill.sHtML


<!-- 参考信息 -->