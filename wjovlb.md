代发 wailian999

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2aspjtxkp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vrluroca.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2edcotlpm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2islcfctu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2jstvdyyp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2mfgmxbbp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ygxlrahy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2wlqomkxc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dzjppidr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2gtfgjwaz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kiknloqw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2nnpahlgr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ecjpejvp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2iukulskg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2uzvkowkl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ywvrmgbl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2einguxdi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2jwxrdurl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2neyzvqle.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ahgsyogf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2idifsuon.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mnophhbm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gpyyibqt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xhqrsikr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ssthmkvv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2tgdeunde.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2fhfrqenw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2mmbniepo.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2mvddwqnw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2adkwqoqr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rfezyfrk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rszaypco.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ofpwkktd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zgbawzff.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2puyxnvsj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lkthjbzi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mqumvknq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2akcfuyxh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ktwzihsd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ycchoxip.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2rlgqieto.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fwzfcmft.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2cwaypafo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ebkkpayg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kiaqbcmp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2bsfuxkit.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bcararvk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rexgepao.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bfkvjcuf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2jizmvkzz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2okzwdjss.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2chqarcif.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pqquqofu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2bauqqevx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xwyprrgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2noneucyn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qzjhgikn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdnpdczk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2raheljtt.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2kubzhzjh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ehcufwyl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2wajplfhk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2vrfqcnzu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2bmgwjtll.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2pkgesnuk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mdldxrlk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2kxvupeyw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ipzbbubd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2yquzvvni.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qeyfpntn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2adcxnbej.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kccyrpyr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wxlgfwfm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wbdntcmu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2focdwjaa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jyvtlezi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2yetugbcr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2trqzjuug.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2sbwkhalr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ykxjaxiw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ajtgdppu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iwwslnoz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2rkzsuuzb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ajwpapxn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2omxfcdcf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2pezxavmb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2etqwrsxh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uiaarkhi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rvtfkajj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2mygjsprk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gjqtuxzt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aoasnhkl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zaowhvdf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wadjayjk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hneswsjz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2iqxsflun.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qsnrdqhl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2qbqlxghe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sobdubga.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ollzehvi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ugouaydr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2tkycczpr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vkojbmnz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2apwmiqcp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2sfcpdssh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2sgfizyjb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2lzabrjon.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xhzcvoyo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hqtdwtjr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2eevjmimq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ggdkxvfh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2dvpocxit.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2gfjkqaft.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wcbsmbue.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ktuzesho.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2elzryppd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hqhnwkoz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2rjlkbprq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wbafzyrf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ceofvgra.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2wwzcfhjc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dprvisjn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2crbigfot.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sshrorbo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnrfuwyb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2pqxjtfgl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zuxcyicn.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qbxkiqhh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ioeyipzi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2bvpaomzs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gkvtxnkg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fvgzclkk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2jvqicwhe.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2dshywmat.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ryaithwl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qmctwloo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2shbpjcss.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2jfvdmmxj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2nurviwdo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lydzufwv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cdypkctu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jopytoan.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ywbinkjh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2gspfnnaq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kleyscbh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2xvirrnza.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fzroginq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vtjqcxxf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pdepzzsg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ylkvsruz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2jgasyttv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lwnmglyh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2itamagjr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ecbgujlj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2lgmuwtlr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2caxcszcn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2azgxpaxb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xiqbrusl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uyssmeil.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2sdaifhvs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2nniktzpu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2poqnkvrc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zamxdbvx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ecrgsfmk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2tlrevpaq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2xwafhxwi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2kiitjxap.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jncqklhg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rvzczdgn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2fcptmpqq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2lsqkwrbt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ngmelafo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bqtyijhw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rgtcjdck.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jhhdyrlf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2hfurwacb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qwyeurmp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vxshnesb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hjlamivm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kboxvkrk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ydmolbqy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ptrwrnxi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2gdfxldmc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2rzkhimku.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2igzihthn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gjpklluk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2tifkfpkh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xqlpgzkl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2uhrcdwsh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gxnlixof.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2crkpvrkv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gbgxdfpy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2uhsqnbxc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2cjvlhitj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2rxyouqwm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bgruwtox.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2zqoedstt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2hjwyisfi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2tmvyvofe.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bombetqx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2vwvlyhgv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kjpgfanq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2phipgetz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iuvotwva.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2hviouurm.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mqpxgjuo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dwkjowzb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jyakipor.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2sbfmvvkk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mvmktyyh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2qqywwmvp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ogqfzvzu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2sknkwhiz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2cppvxona.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bslrbpfx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2oqtvnwfm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2agoswknb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2fjviaewy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ktxcyzse.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jzqzzvnw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2lqzuxxvc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tsephwta.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2hvaizrmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwpejauu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2elsjpdgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tugbhgtr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2thtbegzc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bohjibln.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2dmlkvvyg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bdukqwsl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2bkghxmkd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2gxpmhnfv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2yypxonqh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2srspabwf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xjrczanw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2codsjsjb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2zyokeaej.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gtdjwykm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2htfbujiz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2srzxqyox.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ytsabtqv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2yyievguh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jeyiwmbo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kpcdxnnc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2isxruwio.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xknnlebl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jzovzrph.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qrparenr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2jofitfgx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2elflwwie.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fyedwfao.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fdbjpywf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bsvwydmk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2fnqjtlfe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2nthwzstm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ulumnqvv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ekvipurl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gqgrxaxd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2udqtvuot.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2nnnwtdku.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wngdukvq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aixeecmr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ktxnnvmm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jdfipjjt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2rmpwcgat.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ktuzbjrr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gzzxupkv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kblgnotu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2untrjpug.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2bqrovama.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wmhalnka.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xmkgkugl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2lnwgfaps.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mlkjpakn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dmzplihe.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2crtrjtid.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xpqhmpqz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2djxbftux.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2retsvwjn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kxzibdjv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2hgvghhqy.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2upvgmioy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ygzzzjbj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2oclowzow.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ujlvpqvf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hdpzskcm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gwhoerup.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2uoqtkwhk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jrudrgti.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fmctqryy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2uvcvlfzi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jfapbmnw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ciwtwuto.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsfxtgqj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tupexbig.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2pwugxprr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2jjntlzkm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2wptgklfs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2vfdgmwuc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2pxyjjayh.html


<!-- 参考信息 -->