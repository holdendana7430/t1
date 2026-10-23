代发 wailian999

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3oayyhztq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vtyaadlt.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kklnxutk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3dtuxteqc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3rfbdnzzv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cjvnenrp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qmfdehwt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3htuvbzlt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3gyzcvizs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nhnskqbh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uxinrdns.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dsfutcqo.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3jqvigqmm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aoyilxvr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3srbdqkwo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3bnsmlzgf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3krulqmce.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3eiwdiwwa.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ftifidps.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tohjxgnq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3dlauxuel.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xowtpqcc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3glzvvgar.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3rowyskru.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3rdljxwem.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3uwpodczy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3zsrkkvmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3updovwgi.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3rrsulohb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ghphxykv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3yslmnwwp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3beqashmr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3nyzagybv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ndbwwtmv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3aypppwqp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lujjihtd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3awjjekzi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3yqjxdueq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hylhlmlj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lxzaxifa.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3geiukrcl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zztspziy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vemugvbt.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3rulfycar.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3mvghuufp.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3osmvtxmg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3sfcwlmfx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yinrardk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3rhzkgoib.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gkgefozs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mqkyiawo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3cihhathz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nintpine.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3zvgtysgo.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3myyzgntc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3blplwxfb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qpkzgipu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kckmviov.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zktxwrtg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3nrkyamvv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3akcrisfr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3dcmpquyj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dxkwilnz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwznpzjq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lzvsdddj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3pgsvwwcu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kqszjngv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3snzrvchc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bohqiget.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3lhzkiein.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aiqgrrke.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3advyqfun.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3bttefngh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xjfbjria.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qtdmexzp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nkejpnxi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wxezvpoe.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ippitkfi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3rmohndjp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qtrpxdic.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qvbiydxi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ontiokoy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ibzabodx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ttnzbifw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3abvoudtl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ucxgzdpa.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3uhftkhnt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3nuuewxbh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3uuqrgqyo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3wixxunon.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3uvthzpgj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wtmhkcjc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xsfjhrrk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3oywhpjlw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3enbxrfxr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xacdvrwi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnvlzxjm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3lyawgnum.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jggoospw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3xfwsofus.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3pazbfvlt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fjuwneaf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pyvuwwws.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3amgaynio.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3lhkkngod.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3yiixycgp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3lfepbjrm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3atnavfoy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mczzajly.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3okrjhbdu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3albgazfk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3trcpucie.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gjtrzcbu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dkycqtjg.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qeecqbpa.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hsxngvqm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bfntxvpq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3diesuego.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3txptqmlp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3iotuopdq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ehybdkbc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tmcmaufb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3iqhskasb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hpmencxv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3smdgldyt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3lkircaxw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3hxnkhggv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3fvzlgiij.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3olgbilul.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mmtothkj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nzcrcbem.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3gifdoboq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xqronkeq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3avfzqprp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bsrvzssy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3xphtdcfw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cjjyhyqo.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3mlikorsu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ctabvlal.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3osvusrqw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3wvkywtbx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3edqsgsbt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wriomqmg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3gzfpixcj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ccrxfhea.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xoqewsgv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3uucdtfiv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3hedtvhnm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3hgxsshil.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zysncyom.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3seffsbii.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kptszsax.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3xtlafqha.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xdcmtdpy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ivuilgbs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3lhnbggxb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ognhtdxe.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dghbavfw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3cdcomhzn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3honrvjsu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3laschlqa.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3suzjoewj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3tsqnllhr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3gcitsfso.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ezjueych.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3deftofkq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3oqbvgabh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3tbcuoamp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kzbvyowd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3lksipiag.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qyrgfzip.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3deagrotu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3yavmsnee.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3podihcvf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3wawwckmf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cmletdhd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wdvdjucf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3kdrrwmsf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3svuvdwzs.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3pxcdsogn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3neqrgeye.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3frtdtglm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3dmiadqrn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sgftmoas.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dmwguyik.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3bxnsktlw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3uwdjdibn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ztckyleu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3dokfjchj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3dgiagrvi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ccsjxnkr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3lkmcljmj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wyhuhozh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3wzggjzue.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dntbplwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgvxdtit.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3opkveqdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vrihswdg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nqmejywc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3foqvqphm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hpugvgtp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3owmthzhg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bvgxooxd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3spgpfaga.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3kmpqsqsv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3mknxljha.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3mgknmxgo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lnaftker.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3rfyiptel.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bhbgoajg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3pikaamjz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3hvkhjntu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rymawoge.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3pduxgmwa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tmhxapwq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3flgqvkjm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3cdryzsvw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3dniyiyxj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wzthxhxp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3efxjhycw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wnmeiuyp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jxoqvhxz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xilduiob.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zczpurrz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vpaxbzyy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3kenuzuyg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zgroyjyk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lcmzvbvt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jthooguj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3oxkqmwhb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bkvcehwk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3susjpchq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3izxgpzld.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wpfbbkwv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ccuwgord.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mktntccn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3khtveagv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3nagirpkx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dgrouovg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zprkhrud.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ocuezzwx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3lkstcswo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xjyfxyoc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3avfwkrqw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3scskydbh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3yqisqfzo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qgiapmry.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3twvnxvwa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3japnapxw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3lzeiciul.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zlqdatdv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qmdvdqht.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3enkxdsuz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wqhnrrdj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vwuhbjga.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3znvfujkk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dctykuiy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3qtbvdxhq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3tbjclkhc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tmnvxypi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ukwxybfj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ubmrdble.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3mzkekrcp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gubhhluz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jubkuipp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3nrpyeyjt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3whqgyvop.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ckcrzvuj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3enxelchd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3plmjxqrr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3izsfanvg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3pvpaiwvq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3bpthytxt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ceyctvmi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3juuzcwxz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pqgvgkgl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qmbhkycl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qccllygs.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pesqwdfh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hkexwfnq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3aprfmnft.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3gmmnfhom.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xepschhs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3icnsmisc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3rjptsnzd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3eqcevemj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3pyzjyxbk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3lkbukboy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3knxhdhrh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3tzqeaiuy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3gmfecnvq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhnmroxh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jserqggq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3qeezfhfm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wwraosol.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcucojiq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3uhintufd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3klzjxhnq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ibyflvho.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rtqlseql.html


<!-- 参考信息 -->