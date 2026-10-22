代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jqnldfbg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rwwqsaah.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tymdrxkj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oiradpfy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2lnlyrlwj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mnlrkxql.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2dzqxruzt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2agehdnxu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2oartgeio.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xkagoshe.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vrvjakgt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ccnehnni.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fqxcxubm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rkghmyjv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lswgwrta.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jcpeubwk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bolwrzjw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2kfxckrtt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2mnaobatw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpajbqfh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2axgorclb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uaxfmwda.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2joqsteqw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2wvjxothe.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2dybhuyyi.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ccbavuba.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ugocmaez.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zadpfszk.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hmzetpus.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2xarktnhd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2kkgmxaes.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mbybjqwp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2mnieavxg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cgshcjcm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2atdaamjl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2djvxcvmq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gxvcckmf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2qnvbgmwx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2zhqfmwmk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ritwskts.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2gjvsabtv.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2uskkhxyd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2elrpkqie.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yaipiifn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2vqqrkwzs.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qcymcuiw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nngnpkoe.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2lbxjtkpq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2qjrifkiy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gopdvtrs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2rgwkpjxy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nfrylzpz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tedjrdnx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2mrwbfmyw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hpnmidog.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbvzycyy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zktjzbvr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2fsnhifxa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tziizxud.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2fjqnmtre.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nryvqgnf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rwyqpwnr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bbynewap.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ssuhcsmt.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ufqoexbd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mlzzdzyb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lgahzyyd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uhkoqhuy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2jucwyyki.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ypvzjnec.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2olkvzbzs.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uahfatdk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2elekaduw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2undjceuu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zreoytco.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2rboorxjg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2bfkamoaq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2pknvxwgg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2odcfnyut.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2eavdxzfs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2odsbwwme.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lsaxivra.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rmsxobgn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gmzaanla.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2anedgewr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gegovskn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ihnlpnjl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ypkhpwtu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ljdssuby.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ugqmznae.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehwklpgs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ejhvbzvc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2epdqmycs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2kxcultyi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zbwgqgrr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vjsbqxky.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vuocxaxr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2kwpyujxu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2syrtwyxr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2sqovvknd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzrphrmu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2opxneatq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vuhzampk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2vpmkhvzq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2szztvafe.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2epvirlqx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2szqqdowu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2fygfmncw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nazusnrl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kfqlfpaf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ggndkuiu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ojtlblds.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2qveowpij.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fqkekxwv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2pmzuuyai.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rochdppd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cfwxkwiz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2exyhlhvu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2wpvrcviy.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xfoanmam.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ickhghgt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hjaobmfa.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lzguoirr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2trjjbdrj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2teawkvkh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2eznyvehf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2aberstqt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2qvznfqup.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2klfaanjg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2xcxeslfi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2brtcpnkg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ghskfymx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2vhcflgiq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfzgoygm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2hagstftd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xevcrzhz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2yknkmzww.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rotcsqxa.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hezqkphg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mymfumow.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2nsjlpcie.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2pumovmuk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2sxkukedk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bphbahch.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2pglspheo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wubymwjh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2sdjdpkgr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2rjxzuazh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ozusjzfe.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xdefaruq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2xspegzko.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2woaeysdb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2iakrpfej.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nlsqvbka.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ldefiyxi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2mipdjjrz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lgbpzecc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nmjcbfji.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2iizwjnue.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2gqjlnsbp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gvdtewix.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2rjxkeruc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bwvktmsp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2lbdajyjf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2nunfpmkf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2flsjvuhu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ovkqlwly.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kbuowpwr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2blhqrrcw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2fbzvrcvk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mcvidgvu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2serskpfa.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wbsgjbld.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2krnjnkhq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gzxzctya.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rbvkivnu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vrbbfmxi.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2avtidrpb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mxrrvtxf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2dwsuiurh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2bgdzldaj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2sdzngozp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zjcmzniu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2fbfqwrnl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2chzhmcft.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bibbosvo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xcgkhgcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfadtdds.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fjbwdini.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iropeyyr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dyfmuqbf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2jfqgrgnf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnjhtybe.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rngbmpdf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xsgczlzm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2favyvkgg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2leqgtgcl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2bgxaltzr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pocbqpos.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dagndrtk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2toeutcdl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2iiyggptw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ijujymzj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2svlnrwoa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2zovfxyxw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fkjyjgza.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2tkfnwwqy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2xqlptwwl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vgdptmir.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2enjxfffu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vblxuivx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ispymjuc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rplovzva.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2obzuwuso.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pnxjirph.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kvjsexob.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ihiuvmeh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2kxyjkmlg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ycbbcyhm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2luovfqec.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2asywupbi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ncpmtapv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2hkuqlxee.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2sffmwbsa.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2loyxpgpc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gfiflisd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rymkljnj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hpibeibb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2hpsdjslb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rnotxbqo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wqxdyjgl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vvyfhjms.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qhhirusk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wlxkfgbh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2erwqtdth.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fmnxggms.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hwibbqnl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2nxkxxmes.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2pqithojj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vgzjhilp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2hhcdfxra.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bwlytpzg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2inwudsyu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ooozovkx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wuqpslqv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ysjarlns.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bklnjzzn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ismnjnnm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mrfdblwu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jxjbuhtb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2bhjifzpz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2xvikomjm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2pniwrtiz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tzvqizry.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2nredlhtm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hkhzkqep.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2mgralfhz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qstfqbad.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wxdruvhp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2blywonfj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2tcvzorel.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2npnbwlzn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ujtajxwh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2amctzqke.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ulbpbweo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rbhannqm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lfcbufip.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mmvwedtz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2pemoupqh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jzxxcpaw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2blfwgvee.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jplmwxcy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ugfybkzh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lhjqmtrw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2zaislqmi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2afilimix.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tygwuuku.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jfuareio.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dxwmgmhu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2yoxzhglc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2nufbacxc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2uljsgvac.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2krfjfsmi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jmvaseqj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2twwohodw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2gfnbeoky.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2johviqll.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfdetjne.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fqnvvsqm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ufbxxigu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjportbh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2irdizzvp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ucdkqjad.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mlrpdwmv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hcbexute.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mghnnukw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ofcmmlpy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2bsrmljoe.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2mhicrdfz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2frfpsyaq.html


<!-- 参考信息 -->