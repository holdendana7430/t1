代发 wailian999

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dcespicg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3nbcxzlwa.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vvhuimey.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3eqiamhrz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ocvymnln.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qgnuymxt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cvczgqzw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nyswgfkk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3wpuhewwa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wdpbkjup.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hpxjfiog.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sclxhosm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3rmaciosl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ohfjunhd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3cifyieuy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3taoqhffp.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3iyeajqmz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ltvmpgkc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3quoklkog.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tejjgfes.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3tfnwzqau.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3fuuzuplf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3twyezmhs.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3zvxzdved.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3eiefxcqp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rnslcaoq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qkfatnza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmhfdrdc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tuthctmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tuebqdiu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3msroeexi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3wzlmchoh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ypzorsud.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3nncborko.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3jmgewxev.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3anxfehft.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3satwxicb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3hqdwofpg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3woypqnvc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ihhcwkui.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3rondzpbn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3kstnrzvc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hfzowlmf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3cjxcchan.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3njcutrtc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zbozixrs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uheaojti.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hbcimokx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qhpavczp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3shcymgmj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3npuvucnp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3lywiatyz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tvhoexqw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3aojldxaq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3krzlrive.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zzryipoi.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3sbmmibdm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3lgtdfaua.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3awmctlyb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nhsmsrno.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hnnuzmlx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ooxvnnto.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nhsolpty.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rolsnhcm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dxuymngr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3holhmoan.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ysbasykj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3acwojybp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ynsemxdw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ohwwwzng.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nlprtwin.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rroxbqmt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3klifmjie.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3fxeyelke.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3jlamrgdw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vgjsoaeq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zwebhris.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bcotgovd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3vvzltfpg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bcgywuow.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3fcnqaxvx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ftezxyox.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3pzwitrsm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3eqsbfcyz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3fzcoiylf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rjuhrtaa.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rwqsyyfr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3htothcjf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3fkfzeidg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3vinwwmhc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ptwhfbol.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dttgppgi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bruxkfeq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jlqixnnn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3rhrveulw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qwgssphh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fokvwtgl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3aoqceiyn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zawncnqo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3yczzpsgm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3kxnsxxxt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yqjknrcr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ksmtslnf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fyecyovm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3iyubpwzw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3udnppsgh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ierzchgr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3yhflbwpb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kvjmdcpr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vmaijhks.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3batudzmg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3vetynvbt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jzfifmiw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3avtzunvq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3tkkfgqgf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3krnifwkw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vnjmpwlz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3dppvpoyi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3tzzvfwmi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zovtohbk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3escfiagh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jxnljtfu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ikiquhhc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ednifkjf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nocdkqkz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3fhnnbehj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qhtkpank.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mjkxsnbc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fzcomfjj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3erfdbmtp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wkpbbdzd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3yxqepvyr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ahhlmfck.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3nnqydfdh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3okqpvzjy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lybzxcts.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gygbnycm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ptpokipf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ranqmncl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3rlpqbmrh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jgszfhjw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3huyulthx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3kmflejoz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pxphakcs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3gpoogwat.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3idqrizqv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3loetipeq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3okmfmdpt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hjbxcepc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwfcqhni.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3pplixzjf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uekmadgo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3toalugyg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pvwyimuc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ufknczmp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lnpdszjj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kfqviexo.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3siucgvem.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3duyuetcg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qfvtfbde.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3lhlhryrc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hykjjlnh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3cqhedpol.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ukxcypiv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3yrdsgvjp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3quvsqkjr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jftttwrj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mlprjntu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ziepfzmt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3sxmuepsn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3tzrtjaob.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3jkzrnhqq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nzvzqyxo.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zjfklvec.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3osafifwz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lbbogwhc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3zniabhjb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vhvhpytd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3duhsrqzu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3falrxpko.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ycwgnxcd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3katziamd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qwixrksg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3nqinypve.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zgayhlkc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3maehsjox.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nthhtphv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3gutojilj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3uauehtha.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3fqkgqymk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ypndgkap.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3uiyjxxdo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fplynbhm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3pofkrnzl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3klufmmco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krlaxqcj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3utryovaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwxsevfa.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yjbczgli.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xryfrijy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhwprger.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xnkqiesv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3hblcqgbp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3yavbnugq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ocgasffr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3oxbixlgu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ranhylrj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ulyzbzsp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kqzkgpae.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ddvnmogp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3qeedlotb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ooeiludo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3syrhvmuk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pabzdabq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3atkxgbgg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ojsdjxbo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3atbnvldd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3fnnwodgn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yblzaabn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xydobjji.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jagwjvvm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3obtbihgv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zvpgwhiz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ndtbwfmf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gnihfxjk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ieytdpyv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3wntxbpov.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3mhchdjcj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3gjipjsyr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3anjmovbh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3podendit.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3yeqytqbz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nkvnefkl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wupdjsaq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3xboxzwyn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tmnjnapd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nortwnht.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jbmuiieq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pcvkmrku.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3oqcmuzzt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ifdykuem.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3rfugeaiw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tedxmitp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3awbfctvt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3rfejvrqq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3imqehlpe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3adeikdyi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hyufywcr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3qfwuudgo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3sshjyuzh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3qajkboii.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3bpirkzcy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gnovmkha.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3gevmukjg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uapwuzcr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3mbremwhg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zehiemkn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3izjqpfer.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3mwytvpsk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dfaeqqtp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3tdohgmfv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3bhyoqlqi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3agrqmkqz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lpgufyeo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wsdzpqfv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3klkxhlxo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uwttxkvk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jjatghry.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jjidejhf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uesaguez.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ickuarug.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaffgfez.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3lffrclqt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nbgcgjvk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3epoupjhj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qsnkpisa.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3pzgpzwcq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ejwhnwyo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3uvtjupsm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yazjyqft.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3vxskpzba.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3nyizgtoc.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3qtcqxpsw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xtaqwzpp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xlchegsv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3escjafhg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3srleghzy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wqohmljt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3yelcrnus.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hnjhdgsf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3fstpymmw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3nwywbvds.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3tswogpjr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3rbdxhbaf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3tnxstnse.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgrwdcqc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qvglxkny.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozndqsbh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnqixnub.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3vcgsrscy.html


<!-- 参考信息 -->