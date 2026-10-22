代发 wailian999

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jwwwvuqi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vrsxitnd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2xmdzrkph.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2gyzwevgz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ypmdlhcn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ghujdkmr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2fnwbkxvv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2myqjachl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sgxdztll.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2jxsfgbjz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2leedmfww.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vxpzrhto.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2pdorvgoc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uvschlto.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vhuvhxsp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2fiyixlon.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kpdmhpxx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2scqfrleu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2qzndwdva.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2uckzbgmw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2sbknqpqe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2bgzdpyxd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2snapdnbl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2mmlakugm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jwlhwtur.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lmdipaax.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tffaexfo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2stmbebgw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2emrgwzia.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sgcpmjbg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wayxfkcy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2juebebjf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2weaptyrt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gtsuarsq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2zkgcwyaw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2cjzuispz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2vadubicr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2fqcvugoz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fhfdccsa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2esctmzxc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2hgktezfe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2tuncvcfv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qvlkifkn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2okgvivmg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2raxihfre.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2sfhqxboh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xxytbquh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwtonaoe.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2adorbrys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rafeeath.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2uxvdqtyz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2bqcaefwa.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2bglfuycs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jrmjwqpd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2eahxhmfl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2gdiakgiw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ifrehvpy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2fdortruf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2spvyfokk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2inmjexvz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zegfiaeo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ovtesovd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2iigkibcu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2etwyfrpp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2brputfua.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xdofvslu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rizqdohe.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2albprgqr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jwyksppu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jfarwydf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dsmpkswu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2zmetaikd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2quamonnh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2lfwcbhhc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2vfqhbkzq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2cfsmqczq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2kfidgqot.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wryfgxqh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2otakgjfe.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tbeimitj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2waeuztno.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2zdfzxvzf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kbjkwtnt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lnzvquye.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2uaajqnfi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2aallchsf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xgzuhsos.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hreveawh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2jwjuxtbv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2jkojibqy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2wynqjngj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zwjiiooy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2zqtmgzzb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2npesqlcy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vdwcwked.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jbcxuhsw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2bpdtqrgu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hzeeiwjh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2svxuhxpf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jgiatrdf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2aqmxuctz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ppjghykg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bqxfgque.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qpajnceu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rduyxjss.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ynbigxxz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vpqonjls.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bdmbiptf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ztupsxhw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2zxzziwjc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2edwscyyn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fqvemmqy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ialkjage.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2freilhwl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2klchndjx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2bzmubzpk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfmxstrk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2jmcxalty.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2omnoosfh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vwgwymow.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2pplcbhcc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dspyikxg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tbwqnkem.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fwkmgyih.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2cehnovbs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2jhvfolbq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2llxkpmgs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kkhzotxp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2irljjpbq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mbkslsuj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2mdhdsoms.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2eqmudtlf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xemiubjv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ttqtfkxj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2jaqpgesb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2tbczfebm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2eafgrrxx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2iycnqpfy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ukteqyhd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2foctclsy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2elfcgbhy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ddhntkyj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2nvvrmqsb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lhcchscy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2nqscucus.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ohgpdvov.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2qnvuupop.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fzcrugmj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2woflldhy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qpaofegl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ufndsovx.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2lbnjjdyu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2thgpersx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2bddnkrbd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yubudxzh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2jomgargm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rvygnqsk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2pxtxpfoq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hehtypba.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2auztruqt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xpqrmxyy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jejfoyis.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vzduypih.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2abtwvxvr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ngxtxlun.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2mrgqejrr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2shztdbux.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zedbwouu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2yigvntpx.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2nnbdnbee.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2kmdwujgm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kounkkwj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2tevtgpyo.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pipyuetd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2tmhkbriv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2noyfwzqn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2shmgcqbm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2pngfcggh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ftabgvcy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2epduxtlp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2rtbaczem.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2eaetwugi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2dolamxad.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2bfclewla.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2lbwnvctk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2uzdxjdzy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xifbelfq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2panlhsvt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2yjzlsabg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2bwnfhwrk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xstyrsdq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2cefvmubf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qhaniyoe.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2iwazbhsk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2mphyarjw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mavidtli.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jfxlbfsc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2lhpvejlx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jkzozrtj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2lnwfrscn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2bwnhzogx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2mscsfddj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vvbexbxj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ylmixdgc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jbdrrzwg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zcjwehyk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gwrxaxls.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wjupxyxx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hmhoyivr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2vyisfpbx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2kbtrtgqp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2woskcdex.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2yuujipnm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2vzkxzozz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2iifbfvcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2govrgdbj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fjkeqvrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxadlzng.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eifwrtsx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2uxjmemqh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2uhzoutjd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2pjicbnkb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2lcttduyq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2mpfzblyz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2xiowxxwm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2sojyfcoz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sodcotfk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2sidrphos.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2cfbzsftz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2auobgzfu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lxxmlbit.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2jhrxfyig.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2vhmynufo.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2uhxttcbh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2stxjsoyd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qiwkabsi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2mpmsnwfj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ujpgojlf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jbctsjbu.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rkiyyiud.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2jkhxdqdn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2piizsmgu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fineqncn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ayeayqqa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lnsxfscv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2uglhrjwi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2sbtmqlsu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2qucxqfgs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bmhngqea.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2onlaqeqm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pdvwzjdf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2mliiwuhb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gmwpmgsk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yjwyohha.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2gipfzqqc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wuafksay.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qecnqvkn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2rfpmynmu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yleforsc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xcqucjvk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2udnrvoey.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2neoereqn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2csqpykpn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2bkvefhcv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2clbquobb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bxegrgzv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2pefjbaie.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2oiomiemc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2rfjqqheq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jpqudmue.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2jrbxzzjg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qndtapeo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2mkopyyyy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2sstemaek.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xihnpqkh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2bhpxxqqb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2lfvsfgdg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ixxvdqky.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2bexokfot.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2yzeqwham.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2htjddazp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qugbyvoa.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2pswuujcf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ugzlmaex.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2hrfdhaif.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2icqaolze.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czgfgbvx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tacrqhds.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2aixgzpag.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qgbsbowm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2dmftsekp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eixtqncb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lsksybzh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hxmaldcm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rciydlxo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2knpqxogb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2uamftlpi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2dchrlknr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fjubnhmk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gkmsahjq.html


<!-- 参考信息 -->