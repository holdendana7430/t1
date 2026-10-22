代发 wailian999

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2mjirxnob.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2wwzsryia.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2czcbanif.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2pzkamkks.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2fbebtqvt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mtbulwyi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zdokzjbc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lompgmny.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2kijugymd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yxbcchtn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2neuiwchp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bknknyff.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2uxxvtyfm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zjujpwao.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2hbbuunfb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2wpjigdte.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2yjjnugqh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2uhmkccuc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ywlkvtzg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2blqasamb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2dmtpgzla.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kwhwifdo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2weypkhae.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2smzowpoc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2bwlutqjt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2jukqcepe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2pyyvslfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnspddyh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2cfpiwwug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ksfuyyah.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nmxrxxfq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2wqjfrkvl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2obiwxyqb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2skgsvcsn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2phxpwyjq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2lbfuhhrj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qwcopuor.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2njwrdjhy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2iaseremp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2wpjovrzy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ntkfedyk.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oqjhbccb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qrvfjxjo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2xddetmrz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2jgbddhnp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2nljpxqkc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qhsicuni.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bwmdclfj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aihqddao.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wdinrbvm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xnzakche.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dolxszge.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qksbeuqe.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hnkzkuyi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2aztewcuf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2aopoffnm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2oopymwfr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2lipqmsgk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zvpdxepp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pggxtmpu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pgyxyyse.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2betjqcxw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2krwgwhpv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2puymrcfp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qcxyqgmm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vglzcmqr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hcrgnbvp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2oaywjyxd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ejuynraw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2soecxsle.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fzthxwik.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yqrbobot.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jaavvoeq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2nwewmkhd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hyuwgwmj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ygcgkojr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vtorvjol.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ycemdzmd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ssdbwfjd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jueikbmi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wsgksltp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dnpyrtbk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jniitjjk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2kbolprac.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jhlpdszc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2hisybagk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2yloozpuw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2idvsivle.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mcvspsnx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2smrwhtvq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ytzppccv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2znafshlq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qqzjjgum.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eftwpfpo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hxnbtcex.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wcuhxxwh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xrncxmcn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ntyshbax.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wqadouub.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fogluqpi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xzhhizjl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ibqgarnm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vrjqxfyb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cgemhpaj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2zldewlzj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zhhrjkct.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2vyzgsbre.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mhpdncln.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qhrxetaq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2mzlfpzcf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jshuxukz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2zchlagfu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mczzhxft.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2eawxxcfc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2uzfuvmdm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2dhlocfuj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2iygtjfqr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2gjouzxty.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lrbbgfti.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ciflxerd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2oafiljso.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2cgmxnibg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2azmgyfli.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2nemqfsep.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2aaobbvxe.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ufojcxna.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2iyowlmvr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zifiastp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2smcnvext.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nilwhpbl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qyvdhcbk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2lmuwopub.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2hunuqdds.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zaacvslm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ufzlzfmz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2usvcvjnb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2espjwxop.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2dufrepmr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wrwidmry.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2exrkyfcq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2nfavsrdm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2awfdepqn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2guxlaudz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2qgjxriya.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pxuqxsmu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2liroolyh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2kwubsmas.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mxkxhplr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2arnfdbrm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2fikkkuvo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ripuppel.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wvducszq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zjearjif.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zmlsuiwf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ouvbwuys.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2uzrdvoqf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2szqugpxp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ptsoulyc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2erywwbxf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2njkpscsb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2gdkrrayf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2renfhdel.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2gbipmsxl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zwknupjj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2yhmhiqii.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bwegnrwc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2sdwabjkf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wjgwhvrp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2kqajbpxl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2nbiewrsi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xgmmuhan.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2woaxqyfb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2qraqedky.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2cfvlzpqy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qgrbkjvd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2proemiwe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xrtnjckd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2doilphfx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jwefwzdz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2lkhmzqek.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2eykrjrxt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2gjsziubt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pkvjpiwf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jnolrqnm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2csxhtroy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fgtlzxjy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tgpkpqyr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2epdxagjt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2hzyiomxd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2bfdbxfsw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qdqsgdjw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mwwkngth.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2bbdlsltn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ficznetu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2tdsvbrqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nryiqvte.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2btcbislj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2balbtejx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mdutrepo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2oujgdxua.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2anpvzxdv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zfncszii.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2zgqrgrph.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2bmsbcmnm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qqpmhqie.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2tgrmnbaq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2dmcnyycr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ucztnsnx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iycfbaew.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2iazfongu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2yknlugqp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2uejmjzde.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2lbuxcihs.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ibylvfjb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2whepasyq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2lvvdqflz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2npdjybjy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nvjxxjxu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tjdlfroa.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2thhtlefe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2kscazmpu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uvjqlybq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ebfmoztf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2khqftdta.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jxcgqnth.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kvseoqzg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rfrmrusu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jbivylvt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ppztmifc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yssazlpb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2dticdpzd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2mbckmqcq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2udsmashq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ypikkoxd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2kccqjuiq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bqiffkuk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2rasamytr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2rwaemztm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tentfgwj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2legpplvl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2voheimmr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wpsnqxor.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2crpqdusw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qlxurksl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2eywfgucp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2plpxluae.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2heovpidg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tvrzuajn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2xzbrtwxo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2zdhfsfvh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2dvbqrpnh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2krffyxrz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vltggcjd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2gcqtaexi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fmspekug.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hjjnzgve.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2skwbyirs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2fohmjtyn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2aszkujqr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ocsbfecp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mxviauey.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tyoymqjm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2klskvsbd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mvklnbne.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ifjkmcus.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2kcudyvxm.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zhxoymoz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2raydfnlv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vzjmihcz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2txnwtuzh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2nerlggoe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tkplrjnw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wohxdoim.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qvhubhsi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2uwoifgsg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ufwnlgkw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2tidtroya.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ezmfvoto.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xjyukekr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nnsrkefg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2yxilonhs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2huzxbcfy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2wfueynfr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mrlwolkw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zmfjizmx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2mojkpxuh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dzzxefai.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rnirldwk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lxzcskyu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xujrrbnb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2hwvvtyrz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jnvotikq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wpznkutb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zxoljles.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2mxevasls.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2znrvijgo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2dknsyyha.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2qgyqvzcy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2odrdzina.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2tactogke.html


<!-- 参考信息 -->