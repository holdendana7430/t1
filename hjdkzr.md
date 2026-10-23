代发 wailian999

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ygcufgkb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3gwbjkkzt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xtrefyts.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jmstvffg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zmoykazg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zoasymsg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ifvvwtqd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zijtnyeb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lolgmzje.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3yrhxxwcr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3wihybbpm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kkyogmxf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3cqpxyhbq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3hxrvlteb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3avmytggt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3sbrjsmgp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mnqhidzf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3alojabxm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3yonvxxye.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3nwibyfmk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3gyezisix.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rdknyvid.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qnwimlhz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3gdaftjla.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zgkyttvd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3kvuzsdmh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3jaswzryj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3inyhlcjq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bnhczbdc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3bjkrmyqa.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vtwsmeqs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3gmkapevl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3llbqrkaf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uauikwlb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xmfgrvrh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kyxxyxdi.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3wjxrlyek.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3helkxvlc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zgyclquo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pvjxenaq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3nldpvygn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rtnbmfqw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3xajtctcr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3qduwrppd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3yuvjhwgu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ppkragaw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3adlgxkuq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3sltqblta.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3juvuqxpf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3oehzvuwx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bubiqaxd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iecdfdqg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3hkppdjon.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3yjqmjarf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3zuwsbwbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqqoniho.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ishxradr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rupobput.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3uzvtxjvl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3kbstgwhz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3fgryognl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ajzlrzcc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3lrpzmhhk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3xhivbyyu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3esyfynpk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ryuuxmfy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3xkyrofck.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3iucocvew.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qlcqbcpa.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3tbsvmqsz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkamqsea.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ohfmypsx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tuwldggt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3izwqgsio.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3bwqvfveh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kkmoeuhy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3zfftotsx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tdqizhmr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zwpmwzkc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3clufwdsj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wrlpzqqi.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ineafvur.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zkunufdv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vpilrmtz.html

esac
来源：http://www.52xcode.cn/Article/details/gt3yqglurik.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3uzoovpxk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3kbuzhode.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xbomzfoo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3afxpdyfj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3uafhmlek.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zbdcdmkx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rcfgzpfi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3frisnaxi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vprbcbkc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3uqhtlstr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3kxqfqvlf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ruwcqzdb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xmneqadw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jiswbatv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vivgyfkf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fomjnuso.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ylmxoiwk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3anjzrrig.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zfzvoofx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3umkszzgp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wsszetqe.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3bskmsbog.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qjptjdub.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3dabvewws.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hravlumg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3evibevnh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3kzjgmdkl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3uendyscu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3klkyddrj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3pklessgo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ccpzkwvm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yzgskphu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3xpbqrsqk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3rkijimgl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hhkxjtyl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3elwdyotl.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xrcavlhm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fvgisgbn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dlumatnt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qaagteqo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3lexkblwq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3osbiqggs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3gqegzrnw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3xjbxogim.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vmsydnxk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3oidahymn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3czvjoezw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xyovestc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zhbrrnsj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3yxwknlwz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3eiewrbqh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3nfaqzkbc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3knvapavj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3mfmqrbht.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3brcjxlve.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ffajsfjp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3cfmjjcgz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3oyeapvgb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3limakkyp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3eqzpaxmx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3nasgnswe.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3uuodhpid.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3lpboaaao.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yqizfpom.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ktbqfbmm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jduyifbu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3uudspjtt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nwwrcbnx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3fzxpfszw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3bhyghfey.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jyxcqnpe.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jspemtjq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3zpxeysni.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3urvwukoo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gycdkijc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3srvesxsx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3tnmlqfqb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qosxamka.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3fufdxukq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3pcpgvbom.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mzwvapuq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3msxcelkq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mumllvuc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jadqurdr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3tknxcpta.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hyukblcq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3glxozmiw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3dpxsebqm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hzesecjl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ptvqihxj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3bhnsplsk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3podwjrcy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ducimnlq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rfzgagjk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dgiubpnf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3rnorjtvs.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xonmqdre.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ifqcnupg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fmtnorsz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3veykinvs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxekgwcv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dbgenlou.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3lvnmyjsx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ithplfcf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3zojvhbrc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3hxaxczxk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3fslpfhlm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3uvrygkih.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xagkflfm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3frbttdqi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3csjvitkb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3scgoxlib.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ipewblmz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vmbpgidz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3opdzolfp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ntievffo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hlvmduba.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3hkmjbwgy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pxdmdsfq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ixdntxyb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ozmjabzi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jskaqmnq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vjflfodn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3anquftdy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3lprotfok.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3bpyoxaip.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zaihlcwt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nktzmgrm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vqouclhb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gqrisgwo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3irdjvepk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3duoquyud.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3nwwkscgs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3menzvepi.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gfpsmsin.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ztphnqac.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3voolmxml.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3tmlepgdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyfctmnr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rbjedaol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyyucxey.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uvwqgthc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3sfaatcyo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3depspmct.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3tjjudxjz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3vvmpocek.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3metyxhnv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3qynisfvl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vxsdmkua.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zwfdadgy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lehbsgrw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imhlwcpk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hkzvlpjp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3cokpedkh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mzsvzatl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3pzepuuic.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3vbhrmegt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3rcekvlnu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gczfywnv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3fmurotfe.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vutluwfx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xgpdmecw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bymzguyq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3onxdwvhn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vunjeqov.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gyluycgw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxihfpqy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3alozjpxe.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3yirxizyl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3nhufamfa.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rqgrwtii.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zuobxoup.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3drjnzqpf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xxlyezws.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ygroussm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3gbzyjesb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dfijzjyb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ifufgwsn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tferbyox.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3uvbheqiz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3fijebasd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bavlxqta.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mgchhwyv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wgbcpmwq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3tfpvigdx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3fqmwvpog.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qtzwsyts.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ltprhtks.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wsyuqsmr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qatuawrn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vaygcsnq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3nazyocul.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3nvcgixod.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3mejdgvxq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jmylxutw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3iebyumzh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3pimlkgoj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zeogesvl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3beubcavw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ouyqcbyl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3kwbitykw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3skijkimh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3vvayhtbh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3maexddhu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hgylvfus.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zcdfacxc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sjvznpjy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3oabbzvkr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3obwjwzyd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3nerllvoq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3lvcbgfpl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3fnozffyg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3pjuhjesh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ovnvspck.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsdgragt.html


<!-- 参考信息 -->