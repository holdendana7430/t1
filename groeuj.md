代发 wailian999

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2rcgfkcgo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pbmlavkw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wfhglqxc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mshtufpm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2snldckqy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qbudaczb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ybdqprft.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xyqrudih.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2wdecjqbv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2tmwkvzmx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2zfqcybap.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2afnqkdlm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sgedcrho.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2egtgclzz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2swhnwjjf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2hyfjrfet.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2imrjvdac.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ivnkmoiy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2egioyiku.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hbmhuivw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2fdgzzskz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2gxzypyav.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2xvcqcozl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2lyvvacwr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2indtfnvy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2isxixons.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2iskeczgm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2kqsejxzu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2cgvnbjsa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2biydexmp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uhxidoyj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vzoxtljn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2pitgnruu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vtzrfgcu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2stymztpk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lhoyvdrl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2awrbhubo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2brmffpdo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2gzocrtgx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zavuzwol.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qebujlec.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2bnwbfndo.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ttneuowe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nkskziti.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2sqvdbmke.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2fczlvqhx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tcydxabg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wpuvghec.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2frjggxsw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2quhkgxdc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xkzgsoms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svmoulnj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xcetvxmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojmsywsb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2hfixzrcm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2jnlqvnxq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2pcppsamq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2opfzrckg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2btcykohz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2btiaykrp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2nawjfbrd.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hgtcbisc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2epuhckfk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2alydgvkz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ybmgdxgl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2wkptwdtw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2shpxvbsx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2cpibmufo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ngcmtcdu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zkactzjy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2nbaqmzba.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2savmabaz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rtjfrhzd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ouzymies.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nhdyluza.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ozjeigad.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2iaegpwum.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wrxaippe.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2qkwsfltj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xkkckvfq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xxfamozp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2zfnsfver.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nyofkdeu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rhxhqgmk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ezrhrxlh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2jhoqxggj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fxoabvvh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kmigfwqo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2lnvppyhq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qnvvcnus.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2omyaixjm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2syujldky.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2dpmpknst.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2cqgfglom.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2uhcjzorv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cnxkvyqz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mgmxtyau.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wfmbnmhq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hywtmssv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lodhybbd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2suebbsev.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kqqbgfco.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2venyxzjm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2geotgbpg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2dxkbjzbh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tscibqxi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qklubjap.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2afimcxfs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2nmysqsyd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2fkmqlylw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2iianbfys.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2zcihpedm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vutbkqnf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2laxctqly.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2eojbmqfm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pucxcnil.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2pgzscjpa.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2smthvvgm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2bavkhjpz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vvhamqao.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqmjyyfq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2yfaponyw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xjgkyqgg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qnpcktym.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2yzhbawhw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2odvjczgu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sbopvpzm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ivojzsjv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2btxdlngl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qnfemzox.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2potdevcz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2awpostpx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2bexrojhp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2duexriti.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2dsglogjm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2wzyfawoh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vwbewrrd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2npkezruv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2emlpiuno.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hhzkibin.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zhmociiy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2tavxxctr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2jpzzuziu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2taemzycc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2abftdfew.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2orvbmxuj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kiyihkoe.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rfygyoqq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2bcczxqlf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fnixklze.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2gabhqyli.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kfgsjcfp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2idruvmxb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2eqwlvvgw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xpudqlbm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2gtfrdvhz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2byhplnkf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zljefzjf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gzagcrje.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2sectnfky.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ekmzlgoa.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mdufcfvt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ackdnbty.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2pdrbnyjs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2plzlvkfm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lzgvqvfm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fsclzvan.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mqeztwae.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2voqgmqdq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2wycvspna.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ysuvsnwj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2kdwpunjc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2zxryknbw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hmyhzesm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2efvkqmul.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wejcizmm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2sjvcgwia.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xfkwjslm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2aqqaeknc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2udfnetho.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2pleprdmz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2pztctbuo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2sjdhewxw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2enioahrv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2flaarxow.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2idejzlub.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qbrvkpkm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ndhcnnhz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2bhjcrxmq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2usmtoaea.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2qftqyazy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lzxutmhq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2iazthdpg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hahzdszf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2vmqwhrnt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2lbvawegv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ilfqhjoj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2nzhfvcai.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2bwmpmpcj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eofspjcv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ynycodcq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2utnodbwj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2spycrevy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2fzwpzjcf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2cezorsxj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wboyonco.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2icsgpmog.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2tmeeowgu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2oaoqjbst.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ettenjuh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fgpjzddq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2gackxlcf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2zxgvqelr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2phnkgtea.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2tlahkmlb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2iermcapy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2jpdshvzr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2bdkhutlx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2lnvnwrsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohnvqktz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xphdewfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqxtjble.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wbmembko.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2clrztclx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xacysann.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2fjborasj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qnvnpojh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2uycgbaaa.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2sszaqbfp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2pqnroeca.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ovaikcwv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ncnunbze.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2mjfdvecy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2egztbnsw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2zgusnyia.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2jyhgkjpo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2uldehkbi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2gadexxti.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ybfkolqr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mpylhigu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2qqsvlied.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2bvvwvckq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vkglgnij.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gitwkych.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nwihrgtj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qieixwkk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pxrjotvo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yxffjslr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hkrstple.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2dqwvhaor.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hazykurn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2isiitqfd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2dktuistl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2qejbcwtk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2toxzxztg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2accotipw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2owvrkbxh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bjwaxpvt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dzdbixpd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2shcnbanb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2rkfmjthd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2mwiuinbk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bmcbekvi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2aunrvztc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kcznfpcj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2niusrxbe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2pyiavmyl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lxuqunds.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fsdhobgj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rytdxyvu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2atglqszl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2pzkdjvjj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2rfobewlr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2xzbfvlmz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2aafwmlyn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2glgzuumq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xepdvzzu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2yxcqosac.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vgndzhrd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2qgkwillx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2psxmdpqj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2npkxinue.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tdbmugoh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2uevdomen.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wfrmqsuz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2egjnfohi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ciefbisf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gsttxsxs.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2sxoovxkq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cugdvgrt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ieyptxji.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2dfocbzqi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2olkbbysa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2kjcoocrc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ofmbewre.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzcgwcct.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gjpbhfma.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pypoyerl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2eubmjfhi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2npgdybom.html


<!-- 参考信息 -->