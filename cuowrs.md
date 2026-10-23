代发 wailian999

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3akccuwin.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3wwlrzjwc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3wqgjmrts.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3eyxpxarg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3vldwzubn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zxlkhcuj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xbzillck.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vsjgixjf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3xaqbzxtp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3icxklhby.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3pzardtnv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wmzwmcrl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3cofgxwlg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3bkiakide.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3odxpozxt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3xixagssl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3alevespy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3slosmnwd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3fywbqwzs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ggdbldvx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3miahhbvm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vtbimxte.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xrlkmcbu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3wdaowxkv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xmfdgoyf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ynynyogz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3rcdgyeiq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3nzyxvbxj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zznnfypp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tfssiqzq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pmagbzaj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3vvyhrure.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3wvbleboq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fznlrphe.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3uahtqwul.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jxusclym.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3tqsedjap.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sptqyjbi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3erhpzwzg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nforxrel.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3aeqpkmxt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xqxvtxfd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ubsfqchq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3rhnxuzhr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3dyzndkft.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3omkolzbl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jinmlzlf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3nizjdtyq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ykczpgqv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zovtelts.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bnpwtjlj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3yaadpdmx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bvmqrcba.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zmelauyn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3nxesojbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yozcxujp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3euspgtjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtscppvy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3qngcwsct.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3euqftyck.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vhxileqy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ccnhvxhj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hwptgwoy.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3odesfqgf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3saumnlyt.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3rzmcmmof.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3pfmrrojv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3actixpth.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3hhnfcwwr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fplfanho.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ownjulxv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3wbdvvubp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qroggpud.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gtfhicsf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3xiqnzukr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tobzilyi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qunsoppw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jccmsvmq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ocksvkbs.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3kimontjy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3bwiufgno.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ztwhixks.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3bnoypcgp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vpykbpuu.html

esac
来源：http://www.52xcode.cn/Article/details/gt3rljwtyiq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3wxpjplyf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ddwdemdd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3oimpmtaz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3yidjjfqd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3cjivvpaz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3trdtghcp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3itaifmfg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3clonreuy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3lrgrpplp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3juzwltcn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3pihiehrl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bkxttzyp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3vdiwysqc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wrexbmdw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pftnngug.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ewlqsttl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3cirryhch.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ektyigre.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3phdjvvaq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kokglfmg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zxekzgxs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3bcmtajgh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mibkqfin.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3vdfnxlrm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kkkucpdp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3facnerpf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qdeqrmiu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bmbtzzyh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3xcuipwip.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3clzhnlpe.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qliddfht.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mggsszhz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3kxenqyth.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3wnmvgfni.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tbcpinsx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bozzrhrn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bbagqirg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kcthowze.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hbpzcrum.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3mbmkraar.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ydvkccdz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghtzgecm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3rtfothhw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3oajqvezq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ybygwcuw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3csmurbrr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mrwwlfiq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3olcrttcu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3oyjhioml.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rakaydwp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ceeldvco.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jycfuecb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3rvmiwwub.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3hpqqubsb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3lsfjjegw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sxjwasfz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dhhjtlru.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qomehvdv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3btsluqqi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dcehgtsy.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hblpeoii.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mybdjbfy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ppmfzkpv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3xsvkruxn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hygaxuql.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3uouzhudj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xhqijehx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3rivugwpc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3vtfwsolt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zytkfnba.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3misfunyv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qpkaxpof.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mfwwkkxf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3covvhbel.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dqycelxc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zgyvompx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3eskjenvg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vnmtfbrb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3gjwywazs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ivoknnzk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3jisxmhyq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3agnnzbti.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3gaetfeak.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ixknopvp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uzxnkgjl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3csvondlr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3iyqixucj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qmfznnky.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3fzesborb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bdwfldcb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3zkuyplkx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3pjfbkhhr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3htrhxhgd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3talurixh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wftyskun.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wxbjhwrp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yfuizjil.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3vonksfds.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mkgncegk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ynwtssjg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3pslbkuly.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vpylyzrw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3tiptjnaq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3jxgpuktp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3poakjnis.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3dfynilda.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3tfhcnuod.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3frytuqls.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3nlmhqgup.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3sclfznli.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3dxydmdya.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hyelwebc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3uoldattt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3sxhzhkds.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ojvjeaes.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ofxhmglm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3deedvqwv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3szogmnea.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uklmqglr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3odqtharx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zgriuxpc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yxlrvlwk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mqmwmiqf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3aoyolzjk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zlvyfgfg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3uydpdgtd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kqbcsdjp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3iukslrmc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rifunxsf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3smsnzest.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3lgscrocn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vctayrmf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3hjaiwbru.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3yvstmnlp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3atviyyjy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3raojqxgo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ujbntewj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yruijvvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3excifgvv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3yntfqkhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukwarbcv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cssliuww.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jqpmmkcn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3iigkocoz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dagqffak.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3yelwxynz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3kgrpvjlh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3bxhgjlsz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ukyyidvn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uedvpwuu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ylubqsnl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nigjkhye.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3omwknouq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3mfqubxbp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3lrwpsjox.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gmkmlnan.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xazoagbo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3smipxrmy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3utbaxnmf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vxzfzvpi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ewbmeypa.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qzoqssds.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tpyjgvfe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3gfuljeya.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3moojaunk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gpvccirx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hzgkmhit.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lwmvgxfs.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3btldvtwd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hnbevqcw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3firplxiu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3lflgyvxl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gdvszjge.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3yatczmfa.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zfbnbqdp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ejnuzqqn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3herrxogj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3rnhbdmad.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3iqctpvxb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ojaulhlw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hwbshxrk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3grbgukga.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3cxtblghm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3aiguxnje.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3fwbnjjzi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kgrogxwb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qyhrxcdm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3fkcbgkmq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3nreejyqr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3lshwyxct.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lfzgnemz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3daxiswku.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3egtodpkc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3bglgtjnl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3hhsibuyr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ecmkgzzp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ibqscayu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3exvvujfs.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3qhrlznrq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3aveleypd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rvaurcuo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3lnnwedkh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3swcwjahd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3pfsshevx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3kkjiwezy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3cjpydwky.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wazwpcjq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3npkblugy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3pjeydjdo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3chlcehmg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3oaqmcgeq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3iuqymsnf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ywxtlzkc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3kpfhdbgs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymxwxybq.html


<!-- 参考信息 -->