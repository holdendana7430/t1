代发 wailian999

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2noudyxvu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2nmcicwqp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2lvealgui.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2crtcetdn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ynustvbt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qoxpgkxc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wxzlnnsf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kfczsglx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xfdebpwg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2eivupiup.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2hboxmluk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2jdkfuqoa.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2murqfpjt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2hdfooclz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2eqlddnbl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vdxnrztn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zmmtrzne.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2nnxialev.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qptakgmb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2iwqwgabj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2cykqgquh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2phfcrpzu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hbggdkth.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hcjicdwc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rnodigoj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2xvcwqaei.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dxrxpfxf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2rqbaeehb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pgyvbrxt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ynjnajph.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xuckksze.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2rkeahgrs.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2zknnfjln.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qfjejted.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vgcmvpxy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ffrxrjaq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ipdvupbe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wuwabhee.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zortvldq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2giaqiyvj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2tsybhdaw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2toyokjdx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2cclmpzja.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2epfqelkv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ucfzilyx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2wsbygpru.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2tdzqfgdi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rgmdzpal.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kkbtrahf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ymtmdfkj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wltxtrrn.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2exphmrap.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hrvygeth.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2mmascltj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2bnjecezf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufurhvuz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qfujetyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tijsotof.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2lotloisg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2jsbgxdxn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2klxvllcl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2aemzjzyq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2sbotwpbs.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2wrofaoyi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2sgupjrif.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qfttnipi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2btyhdeqw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xfqydrmb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2raihuibm.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2foavkhwi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ximvzqas.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2iblumttl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ennmbzlg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2imxnaksj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jwqlxtkz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2toncadft.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vdxcyonu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2othgxpum.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jqgpifax.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dbgaxlqo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dfgjqonk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zafqzfic.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2fdmzchxc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rbfvgqmp.html

esac
来源：http://www.52xcode.cn/Article/details/gt2yrjnldfr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2sejgguue.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fynnzwac.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zcnpylmn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vaqorylh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2dhagvlhm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wyxxqfxs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dizfpnuw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zfoijrnw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2behvtdku.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hbzwdwbn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qwgsncsi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qbsaeukk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ekobawxc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2nbkgqzvp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dssijuvt.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2roggpxnb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2autgbiro.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tsclrhko.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rqcajflv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2hlnifugz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2elsdvcna.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jxoqpaut.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lubhhjxq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2nvcoykdy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vlxzskaz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2twzavopa.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wembwmrx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vaqfoeag.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2czvxqido.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cybvzqeh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gtyqlqzh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xxfengbh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2yrlbbmkr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2npetmofq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cnowlttb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2twwxgajz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2nqhijyqn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2frsakltr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2txzqgrfx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwqwpcwk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2griczvos.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jdgyzrvk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2uyvaobxu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rkqlkbef.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2tbxggcaw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dhlybsuy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qdrgibmb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mtclukzh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zojpczps.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qjweihmz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2bwldschx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhchailv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2dxgdvoxs.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2hirbmwqv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lfmwpkej.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pxmobdne.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jgvehwxh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2bistzodo.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2usrqitez.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ukpjzraw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2oufbpqte.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2fxisdwkk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtwxdqud.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kqilxzxy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2qfegejpm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2njufpcqq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rtfcxsyv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2nbuvdjdz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2uueqwwtm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2fntrjbgw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2yqtcaulq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bvztiwxo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ktryiorg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pkylzfqb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2arfcjpvt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ttgzmlyi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2dpnfugyk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bcporiyd.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xdviqeko.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jxeajszs.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2elnmujql.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rggmsftu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2mbgdmonk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lpqnbaeb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2tmmmnver.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iohsauvw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ozspmqqh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zmqbvpsz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jfqbjnxn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2vrzpxdxa.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mvhkoven.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2pksvvngh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2qmcsdkdn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2fpcdftna.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fnicfsnt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2mkrskuqd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xtifpgug.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2grfkbcwu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vsowwgxj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2cqfwcwiy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2umnebbvz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ijvjyslz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2efhkqzsq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2hxyzkggk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2jddcgxxk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pmvqdzzz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hguffkzh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2sqpwixbk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vcrynjwl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2acupbxfp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2yrtsvkzs.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2sckygwiz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2iaihoinl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2bwoofwxd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2arjkrfsk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2xhufmgha.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2olzogdot.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2neeimtwq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2whbjyutu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2pjxlsvbq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2sakckare.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vmdewvbq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2lffqhqbe.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2yperpisd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lpagxnuu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xzqzvxys.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2uxxmvhcf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2flsadqif.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2isxmwmly.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2opnusnjl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2oaldqunk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2pdyaugxf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2imokoofl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2uuusquyy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2vslpfqci.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2czhilotw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lzenbooo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2eiiljmlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehgizivj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wjznanwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrkxmvjp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2liazjjyg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wijhhsfb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mrnagzfc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2itfxybbf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2lwkegeyl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2uzyhdogr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2uwxjfnnz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2clwapccq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mpjfdxja.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mnxhhhub.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2cwvgdvca.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ktygjogy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dazvhfop.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2xfpanjad.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2lmfzklor.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2jlhmxlqz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fohogedf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dtoabwuq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xwwspofx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ganpqtnj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2eqynyytj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2boahaevg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2qtchxuxe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dfwhhsii.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ktmgvahw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2zivirfoh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2galrykat.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xfydkvbr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2lgrtfebi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kmwppflu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2uvnbeqwm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wbzcbkvp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wqcnuxvl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2qgimzmsl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lftbnulc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cumejrxr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2mpqtqmsi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fpenqypl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jotkocgf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2bggdpmse.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2edkqjksj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kfkyaiar.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yrusceru.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kfdeynlh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2axzdopsh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lkmkjagg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2tgyaajby.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ainwjoks.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yazzvdey.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mhqjlikx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ujawybrc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nkmjgfdz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ejgddqrg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rrntupul.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2jupyfzyb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2oneihpxi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yadermvb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2axntrdvx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ldbqmyqq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2nbndieov.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ibwbjddf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2kavuaekd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2oxavqlho.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jzxeywdy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2qfnpoijy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nhxjqgyf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qecnwamj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2dchpvpaz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vfvliili.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2oijuufbi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2geoqtccc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gmtxocry.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2kusddwqc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2uyavguwn.html


<!-- 参考信息 -->