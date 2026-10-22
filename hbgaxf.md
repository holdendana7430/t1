代发 wailian999

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ccfqutzx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2vnonrnll.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2zaomcaga.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2hozmazmw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ruymyddv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ezzdhrdr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ohkynuhl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nhvqnjsf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2fnxtvden.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uizbexyb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xhezhtjp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vsurahhs.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2zxikkszk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2beurdbov.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2xvkoetns.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2jfvrucod.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2dgdfgkuq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2oofythla.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2igplgjlq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2oqgdskow.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2lcqgzzbd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rbmyvwpk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kwlqxxvz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rnnbfyvk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2amknpduo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dcptoiws.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ytwzftrm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tgloymez.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2opucnrqy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zsojbofa.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ueulmmre.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2kojgcyvs.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2vcfnpnmn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kkdgkgjt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2yhgsdcwa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2mpznhpbf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2snhmnqfx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2slmygawa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ujtevltc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2muzdcgrf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2zplaijhm.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2rhyjgihg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xkblnkvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtqzxjxu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2xvwatgxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cycywjkr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2mbaktesb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2dxafwzpm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2kuhrxjwu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2brjzubla.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lnrqfrau.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qvdylvhq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ogxhcduj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ccvaorxf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2snxoveui.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rguxqxwp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2bmqatntj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wsttscqz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ehvepzaj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxzauwqk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vpxtyvrh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mntlades.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2eoowhnkp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uqifddbg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sbltnnpy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qemhcnce.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rmifzbjz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2hwomqnhg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2odbfjdsf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xkgbkwiy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2enkaekvn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2zgukvafq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2hxobguvp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2elnejfkk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2usnbymio.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vpkvprfj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kyoqoxyq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tqwdafcj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bybqkrwp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ecxraxrz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eacvlrqg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2aatycclg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bkjvdimg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nobalwpe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qwptaugb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2kyyfholu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fcegwymo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bcxpbncj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mtvhgyxi.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2kggrthjx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2eqikuryv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wqjkebzz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hwgxiknv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ukbrgqfh.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jagmlsdi.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qxtqolbu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2skdoatue.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rkccnhhl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2uveczvlt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2htessdbz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2jnebrjqc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2hbppiiyq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2qnqgfotm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2fsxsgzef.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yrpxuokd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2bwyinqiq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2camtkkjc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gmvudpwn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ljwmfczv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lgufltqn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gxuweiuf.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2mqkmesjk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2jbxdiwnv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xuzhtgea.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kclbhpts.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2frvxsxef.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ybanemye.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2bbnnqtwc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ezahpxag.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2jwiioctb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ldfvlybn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ruwdicwa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2moujjazn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2swdkinaf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ehvnoprh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2kctgkmpb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vpiyroab.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tnydjzub.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xlxudmul.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mbnsrjld.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ajztnjhq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2acfqdwuj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2geyqtjwb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ycdljltp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qnwhzwvb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2emczdlbo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wyfbftgj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2bkcixwsd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ggmigvrf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2hfjagsbf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2nxbowsvt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2oggsmnld.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zymluuwx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2zpayuxvl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ejzljrqx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yrnvglev.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jfrqpabr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2zranqorv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2hwqnbujf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vleygkes.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kwtcczeg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2uknvrklh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qtwfiukq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2iatcxhon.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2fuqeails.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2gzhpbend.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xlnkfamz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xcrtanqa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pibpwjmc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jdjouzni.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2uwwgrcms.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wazlmugp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ttmfuaqg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ptkzkyug.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2angvpalr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2qeilvwbf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ftkrdwuk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jyydxakf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2tlttbnst.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2joqxwlok.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ndsvrjbt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ycdssvaj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dcprepgd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2frcdjcli.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2gfvaialt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2nlqmarta.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2qfirglxx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2aorkmtyk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2abeaecle.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2csgkbkmb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ozttfdsa.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2njtxtiun.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zigzrjqd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vldonges.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2pvrukdri.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kxkbizjk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jevpqtkh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wlkpwzpl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2fzwvhksm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wutztxlh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2oldfvvez.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ykudprsy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zsvseilk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ykosvjps.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ekhtlveb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2hbzdkcwl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2scvofemq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2choepass.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2dbtmxhwx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fsusvnrw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2gixgvqqf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2cvhearov.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ifuvskzf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2msnatzfk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ynskszle.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dyatrwng.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qybwitdh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hmsfczxb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2glhhzbsi.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2witwdgcg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2wkgcdnlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzutboil.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2saxortqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmeqwrug.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lgwwozpi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ewegriyj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rkwkssqz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2garbhkzd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2zsmwlvlc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2foujdmbb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2tnmpcecn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2oxzxbvop.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2horntphx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fpqjhfhz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sbmrfywx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bmgxgjdm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ppmyensk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pstcnumn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zgsaoomd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2cnghjlqp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rtjnqyfn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zzegdtzl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2gtqvujbt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zgkntibt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2oosuuogt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tzinbxwk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gqoeztsk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ioywljrd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wmmqwqfw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2sulcwrby.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tjszbkca.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2klormgbo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2loicjpah.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ttkrcobq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2xigldurt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lbaullde.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2apgnwuao.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rupwjtxe.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aytbziio.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pwypqmwa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2pqfmpbxk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zfwqqeei.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2eqaqtdpy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2obsjbder.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2spxfotrn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2nortwzvs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2aflsljce.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ngqkphta.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2eceynuhg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zphqeixu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2zodkqqga.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2tnmfeysu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hfwfofuv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hgnrhxzn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2hzsvfjlw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2klvzzwzb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2cftwsajs.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2uxbxneec.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2mtwjzjnd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2biiwtgqj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2posmxcst.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jybyjxbt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qjbskbcq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fudltmhb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2hahkuvez.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2hvzqmruq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wiwkmmam.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hmgpdgfn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2adavgqix.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2curycrox.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2emcdurmx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxovuolg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lmolqyfe.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2qowjergs.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2jhsoxnjz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2iipmcjwi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2oiqdgmol.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ikuoihqv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2chysalqz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2imtudpoy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2etotzusz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gcpkhzbl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2weighlfw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qzvwbfma.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vvgqtefx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ksrewccs.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ohbftfgj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2pzqodser.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2opseffqz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mehtkgvg.html


<!-- 参考信息 -->