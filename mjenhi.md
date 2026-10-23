代发 wailian999

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3nsfoueip.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zohveepw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ytyjmsgg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ubnhaejg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3evgzgaef.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lamoldip.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kelqowuv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3byyoxejt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3pdtbdgcz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jylwyzdu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vejymnrw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yjxpxpgn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wxmlvbdl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tadvaixy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3idshlsno.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3fvckblyg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3tkllfonf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3cnnrqmpq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3scglqhht.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3gszvnyiu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cbdlafxn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3nlzqazor.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yiktmrvx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3egwpxyyh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3jtqoqbiz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3yfdcdhrz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3amtvyzty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pajlhile.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xcplqivq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhxvibxf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xkjixqef.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3hurdabxo.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3lfvcfbzb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3eyjxcviw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3utqkxwyw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ntpsttgj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3adbbyyxi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3uhcmuqth.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3xipkaads.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jxzequfs.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3evpxcoob.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mqtueglj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3apmkvkvh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3yinjfjup.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qvjkhzhh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3pspfjtoi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rogjuyle.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3noydzppz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3guqhynpa.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3xdjypyrp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yksjriia.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ihuzixmv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ysinraaf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bbrjyfth.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ymqjuyvj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xfssffby.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ijiiszcy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3yposgnlu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3oebjhdqf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ctatjstp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bqkbpuqq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3lmdwbgmj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ztqycofd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dovyynxf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qxdaqlgz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3coqjjzym.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zscebiwj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3jbwzngkh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3sunviblj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3nasoszgf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tvezxejm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dszbmxhk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3igvxgvyn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3oxlwanhi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3omqfjitq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vihvttvs.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3rhnedoqb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jxbqnrpr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3jeytefng.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hiwqypfs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3jiicywqc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ysdbocjl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3phtlgzoh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ejoykkoc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3gwomzbvo.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jqoqggtf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3hmbfabbr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3cosfjrjk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wvkdtfbv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3hxwpxyuo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3czqsowrn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ydcjadcp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ciwtzedv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3jsehgiye.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ecvhgnel.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ucacvaof.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3utbczhgw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ugbbrbyn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ocdhwoxu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fdmxbxid.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qcrezpkm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3cccqeumx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yogguheo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3pcgwmobn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3jxiasxyh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3hpstpjxl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3szalhecc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ixqfcfgt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qhppdbkr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3szbyntus.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3oklghefe.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3vwidjewu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vikjqlfq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3aynmocrs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ljwbrdvf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3lvgpniac.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xbljgsnq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3tpkmtckd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lakxrueh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmqqneom.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fhqudfbb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kwlegoas.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3lwximvsy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ufctvnih.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ofzzzjyk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3jyyjxmdt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qicpuitj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3yxtqlwwd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ijsmlyrf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ljlvyphy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gocggmgu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3aladfsto.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pcpohegh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3upmhriza.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hmjhmpfm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ptcwwxlp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gkfncaqr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3eppdyfei.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kbamdpnv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3msqlfelq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qucljddl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3apjgubvo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pcruhirg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vmbrbamp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3gezvqzyx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3bsawzevk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ljrwrlsa.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3yzxbpskh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gxmtvzwl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wnbpfbbz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3xrjiftaw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ryprbose.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ifwjiaqw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fxhrbkfg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3nrrifcja.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3lztekemc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fhjizzaf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3eifpzukd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vdthqfsh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3jeanbvnk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3uzcuqzhy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bqqmqgtt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3dsdbnsdm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3vvqyrjtn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nqayvprd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ubahgrpp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ewuqxafy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3pumouehp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kwcrwvos.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3luhcgohf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ngpvzvra.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3orhgeccu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3rqexfwyu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3dgobfxyq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3reslgmzx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3eyomnajs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3fswyrjba.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3txizabhk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dfevozyr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3dqicinpg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3pmhmcjzi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3lpafjihu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vvvlxbhp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jznlxgzo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3jfuwbtha.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3yjvxemmz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fwxstgux.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dxysladk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vevmiccb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3vbvxbhge.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3idcxlqrv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3idfzlzic.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3exowwdqs.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3fzsnfmek.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hcjhubum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrzvgvuj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nxrnwwnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmxbzxwb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gbalikeg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ytsezbbu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwbbhuub.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kpobuooe.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nikpekfh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3otawiqvv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3otsozyqg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ayeqreyd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wthoopqy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tooqkzsj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gsyliwxd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tcdflvml.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kccsrkix.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3yoqbbjtm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3dggtcuns.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3uhczfvmb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qwxryngv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jqujxhvg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3tgksftdn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ofkhmbhj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dfjwzdfz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tgiqqkwn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qgymagvb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wiotyiwi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dxmrjfqu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vodjdljp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jcupbeqq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3jerzmgji.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3axkhsnfi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3dcenlwos.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3xxembwec.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3yamrkhgp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3zgiycvzv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3uhkfsftz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3tibwhksy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hnppgjex.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ulhflufc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nkwjgcwz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3tqthqzca.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3vlzuvofg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xzphcagx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3fsirdpan.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rdjetvck.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3mzsribxy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3htstvwop.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qjieblew.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3uxriclsr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fohpsohf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gjfropbm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ptedphvq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3nfqjtkbs.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qxopjzro.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zbfkbxqf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3gppcmnse.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3okaalheo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ayrbithw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ajcfonwj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3fiehpbkm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vkgzjbvc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vbvkobar.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3dxqdcxjn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3lfasmwxf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3szzjejdj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qzzqohzc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3logopxxx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3msejmsft.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3gpldocga.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3mhgmchse.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rfozxbjr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3gzqwgits.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3iuqxfijh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jgaudrjm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3obqrzyia.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfiyttmt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3qwhegytl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3idfcwumn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gncbizdz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3exbxacxo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3aumlfbmm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3umqsmejl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vtmqrrep.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3oytpkymw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3hiicuzuh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fuaplnfz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3tyfudnci.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3holvusgt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nyihvbvf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3npeayzqj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3gbtxqizy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3vnaljabw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ygewkbpd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3naclooov.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3cvgfnjww.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkqzrsdd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vhykyurj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3rfgpgbir.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3rbwgioev.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xnaublni.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3igqkhsqq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpkjwsdg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wfjxumbs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3fgphsukb.html


<!-- 参考信息 -->