代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2qdafecmf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qmfucvvf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ehmkuzsb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lpbhpnic.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2fpjkioaq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vbwdkgcb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2jagzncjg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ctfamkbn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2dyhhblbp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2swarvcce.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2rjpeeown.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2dztircdj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2nicvlctd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2olzrupsb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qlrevwld.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xnlhggfi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2orhowwqf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2jgqinltn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2lrjqpleq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apkrpusf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ehecflwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvmpydlz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2kdeedavw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lfsnqxmu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2jvwdhldv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2zrvwisda.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nejjqrla.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2vdisugls.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2fmqijlff.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2juyyoblo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zfwwhniq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yvezcrrd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qkqyldka.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bshyleuq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pqwqzicq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ehmmmpeu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nlxxevci.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2dyxpxgfy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vgazyylm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ebyjavws.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2byutaxff.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2nippthwf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tzdqstjv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2bmpzabyb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2pwjiaxli.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hdfeefpz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rwddhazm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dfipyqsi.html

esac
来源：http://www.52xcode.cn/Article/details/gt2pizmmbef.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ibftaivq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2prifemfm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ixrnaeii.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dwoswfxd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ktvxbxfy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ttvztiza.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qzrodvok.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xebrcxbx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lamegyqo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2cdlwcztz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2fpwrenct.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mgacliwk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zpgmlwbe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tatyngiy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nrnwkyke.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hdcuivkt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qupwvgut.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2cynglktx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2etlthide.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vlmxcpbg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2efhcormb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2hqliwtmw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ilimipoa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kivbgnvt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zowmwwjs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2legynqoi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xkohzfwj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ntyyknrw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2tfzkqzop.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2blywmiqs.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2lsqospkr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2urswwejf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xekgxhrm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2tpgukfkp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2khjdlyvo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2neavuqlh.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wfiiianz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2abgfgunw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vqiiakyz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdjclsxr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2zgchwujh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lyjvlikb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2odrlhzly.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hhgwcvby.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2tbluklnl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gjtklqum.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2tseqsuod.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nrnziuci.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2mmwqgkaf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ddeffvsw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lxgfgqbs.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wlabldla.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qjrdnajd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2iqymhnxa.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2dmkzuwec.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wmvavfxd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jaykzmgc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qgxrpkuz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2pfogohoe.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dhhsukow.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2yifdbyfn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sxxjqblx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2bfdkuyit.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2crtiquvm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hlzdtjnx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2slwhozqw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2hcyrrlmu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2aawhbqkc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2rmbhvamg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2sjyoppsj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2nkvjqcwt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2udbgwfef.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2clqutcoo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lpvwbmpz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2fhawhnjz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2yzxpmjtr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2jidemziy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jmkbnvvv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rdlrqstj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jklfkzjr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qafjdbja.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ayqcybos.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wopgpemf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ajwdlueo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uyzkaijx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2vqezmjed.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gpuoezvb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2cfswmqyf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2wxjcxdhw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lrjusrpn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2awooshqq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2rchnnhhb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ajosebnn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2kltxorcv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dquioxik.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2yajfryoh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eelorxqt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2zrvuhpwp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2gfgwozem.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2jvjzcgfq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2yjeyfogg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2giassfgd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kkvbkqbb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2lsskwklq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ntfaqsff.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2rrgimokr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ovhromcj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2oimynwxu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2pibougah.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ssfmirmg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2uibhyndh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2bctrihgs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2pjlojyxf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ytsskmfs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2iylvbdkz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vladgpyx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lzuovzob.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2onawfcwp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dipoecws.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2scytuerm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xeyfnrwn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2owxwglif.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2wfxhbvhw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ldorlgys.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2noeufspv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2seixvvdh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yqadjhul.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2uknhcteg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2fjsmfsoh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qanarpij.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ggrcsppm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2mfuxsvux.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ssqksiaq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2pludzrsc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2rxcgcome.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2nqfpljrp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2zeqkhgks.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gowphaem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knkzkfcp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vznffwab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wazzxaia.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uzezzgkg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2gprleops.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bckkebwz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2aeylwicb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ivejrukj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2wpcvfqcu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2xgbhdnhx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2icpabwad.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vhpbyldi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2icvucosz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2rjxqyprw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2sjcsacmy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bzqtlnbk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2bbikqwih.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2fxnkkemg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2nhzkapgn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2eajxwalq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gecbtrdd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fhqyofgr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ucnhhfuv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2lxhcekdl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxnkgcel.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2uljaxbbb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tuuhynka.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vvfbparw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2eelydjvw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lhasdfam.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2bxasjvlm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ynzivzxt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mxlabnax.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2wczmzdut.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rplyvwdw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2lodxafru.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2tilbellz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2kpyzqyis.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2crcbehao.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2njcrttxj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hsulxgxq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2miwtpegx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2gpsoordq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qqirjbpl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2uxmvfsvx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cowzbetx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2pcdcokzu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2spvchmwr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pkkeajvy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ozeiubwi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pbpcrhdn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2mzzcslfb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2teyhhdxz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2cnyfnchk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gsvkfwlf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2jfkrubld.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2uaqdhnzh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ipqumbjr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2whvrilnr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2imrkxdhb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vjvgumps.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2fjdjpjgp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2lmvyctsr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2sgclezdg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2yvrtietc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ubuvdsjx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2knujgrqb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2tkckkwok.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qooyhkkg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cxemnekk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiuhgmod.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2axcrtmkf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2wukjisoe.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gwgrlifx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2drpxgwvn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2qxyojwvn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2rqxmsaiq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pglkaqtw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tcfitmsr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2luuaiujx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nmamgzvt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2sdxmklck.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kogrdtlr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2nlmchcea.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xnjydyws.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2hnvmksql.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2tdsesduy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2uhmhgfil.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2vqlxpmso.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2cagfbzac.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kzrhudbk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2seylxpwn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2dnbqeuew.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hdfpfdkn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mborpazr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2tgwgeqad.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbjktwjz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2cuzqcqle.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2nynqmzxw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2osneplkf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2opkbrclt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kdkpxyjc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2fuvcfxze.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hkxinyam.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2tfnpfipp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xbtqgubn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2nzefvkcf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rdtqkpbo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2kdtemtdh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xqmermqi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2chlidamc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2whwvcedi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2bqfising.html


<!-- 参考信息 -->