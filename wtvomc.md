代发 wailian999

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3hvytpgjp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hyaavwsr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jujiqfnc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3culmhvqf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3wnqvbcqv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dlnpzvep.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rzozwdyj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3apyhoxgs.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rnujxkkd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lbzujzzv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dinkrchh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wkomvudf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wxjmvssr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aiwmidjx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3mfffyjhq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3hbrosgax.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3xtjdrvcm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ejmccjej.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rlitwzye.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3shnitqmc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cnqsxpdy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3upgxgpsp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xgoiszpt.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3uvecvlxq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3htdguqgz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3fulznipg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3zjvjqaea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzysqmxy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zxfjzilp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgvgispr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3yirecmub.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3mungpgql.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3jvqovkmi.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3eimevina.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dlphwnhs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3evapnqig.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xyhdhkbw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ogvjtnov.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jwwpczai.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3bqvlszep.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3woqbosbe.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vezmnyxv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gwbnmiqu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ikyxpsux.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3bdweakxc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jbcgruud.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3embzdiny.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vbinpbey.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ljlhwkbe.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nsrdtzzm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3skfkrgyj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3fzunioqs.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zkwzyoro.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3oniuvuph.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3gtxzrxyh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vpsavpul.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pkxjvvla.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ftuiqexg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iipszbva.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3iuvmdunz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uowhqepb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tbwzfmdh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bwxydian.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ayilrefh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qdhdjrfy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3gxnrapad.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3chqgbbqw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3fralghzz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3dowajhzs.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ibbkgdol.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ubztvuau.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ykgdlcjs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ayvdrtug.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ararwfdm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3tpimlcrt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zyvtnufq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ejsxpqgx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fqeeokur.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ivfubkib.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vhkgoxly.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3gqacmwmr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qefjhfui.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3fyfqdfye.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hdosjdnf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ulktzghr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3eacvljcs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fxkfdaka.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3iddcpicq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zpnhzfgp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3guselndt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vydmlvco.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mikvxbdh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3zgdheugt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rtnywtje.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3suoubaaz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3txbpuyng.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qkdspwls.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tfwyvfvb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fdzjinhi.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3cjuzpveh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3oyucxyor.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ftyumrhd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tvaropgp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3poqlmghf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3pcwqhurb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3derjzxcb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3dkvyqmbq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3uneqfmku.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zbbmsuzc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ofgsppbg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rimkpurq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ltbbhjjk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vqfiydpl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3yflkoyol.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xzpractl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3xvqduxjb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fmjwmytx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3elqudsec.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uyshuiwe.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlirsmna.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3owihmtkl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3mufilbia.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3sjpssrqz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3oukvexec.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3obwcwugl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3nudprfoi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qkfoatdu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3phieguba.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lcbwcnyg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qwvttmkz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kstptdfw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ilonrnem.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qabqrmwc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ckafgsam.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jmpouocz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ficmyrll.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3xjeguywa.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3kjswjdxs.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3iyajkbjp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3yuoheuqs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3tmoltwjz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3uvnpqtqr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3rugjmhqp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3xufmfudk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3trvbxdkr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3sgawlvhu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3zzbwqgzt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3nmhuqjle.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3bvaogunv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3smzxygow.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dznejrgq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3gtxzbhzf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3goxngnxd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yhdsityg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3hjcxdwhs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3loespcvj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3nkwthpql.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3mphyparr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3hagluokp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3sntlpmjt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3istfestb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mtvvnuck.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ayplvvrk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3habtanjc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3vharovzv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3abiiunkr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jtylmskr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3hssadhss.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3elhcbsau.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3elvibgpk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3kcudjcxz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ztjpogqe.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ffwepauj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ibviqnau.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3eldzikyl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yuiwauqp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3cwaacqbg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3iigtitmm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ydaconur.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3voehrwof.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3oaodgcjx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3sirbduds.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ymolfssf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jljlrwwe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ugdmpudy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3txhzwsfm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jyrobrjs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bndazejh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3mivkewzi.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ujnsrnze.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ugrcaqnm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3chostyzz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3mbctmtix.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3anlynczm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3jlfzdems.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmczzedf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3muwanoje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjkcctjl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pflamlcb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3sldknomw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3prluzwxn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3urnutsjz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3jtfvxqre.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ewqkqutq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3vltsnqzw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gbhckedj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3lqxicqun.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vzmapmcq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3naxpacoh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lhvfsqva.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3osyjxkkm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3gtgtodbo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3slnykttu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3xqjvsixv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3gyuwkvil.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3grgtklwi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3pghezrvo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3cyikehkc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3amgoyfwn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3enhsojtk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3bewisamv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3inhpyozf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hxrytgdk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3mrrdtivo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hagrzhwo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3oanogybg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vxopuvme.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3cnuwesjo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xoplqnry.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sjoxgmtg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3lrwembbn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3gisizwgd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3lcrjrgai.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rdzjcgse.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3oqomparh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tgrmzjcg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3agmjgxet.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3jhuhuhhu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cojevooo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3swbukhby.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lakfmboa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ifmtrsyk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dokqbcpx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gcyixrlv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3luvpzgwh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3atdcjotv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3bknsjsic.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ytxxufyu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jwieptdw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pdigjldg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3cmgwvauj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tbtqxwbj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3cutcwbbe.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3bfphtntq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rfplkdyq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3twbktons.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wjxosszo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wfjhkkmj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3iircnvka.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hhbygtrm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hczuzcrx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3bgjdkerw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3psrbehoq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zrjrxcnb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3dowitlsc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rgyfeamu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mfqlklma.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3amnabegc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3pxssnqkf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zqqneokr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3uvvletjm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ywsuokcx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3keoxkzqq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3czwblmps.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lmqigddj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wyvgzqim.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3jhjjzgtt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kqgahspz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3tkuhepnc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jhauetbo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3pnhfrgbe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ynmyrnro.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3nhfunmkq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3oizohtqg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xtssydde.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3bmaejgid.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3umzleedj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fdemtmxh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3njtgyxjy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lwwrgulm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3shkytkju.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vquogvyf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nabsyoto.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3jegcvqrv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3grxnjoqx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kufpioct.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tjsmozhq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dobovbaq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zcyjgerl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vfrszoin.html


<!-- 参考信息 -->