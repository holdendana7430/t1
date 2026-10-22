代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jguiltlo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lndjiznj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wpunmopy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ilasjogz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2udsrszcb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cyxbojll.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zxddctyl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2gpdycdsu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wkmsunhf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vdujqkcj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vwpktscl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2sxvecyzz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2oasjrxdz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ihqefwna.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zfkyaubo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lcfonsqo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nugmzjuh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2jmefpftc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2nwvvinou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fssrfmcj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jyqvplqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfbnswvs.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2tgeosqpp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2gvqrzvqq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ghmzgcye.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2yzlvshgw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ybwclsbo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2yvowwldr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2vzlvkrmk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2edcreqcg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ppkwowdj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2etgjwlop.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2tadzmfex.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zvgislyo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hklnojfw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2daxdwlru.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2syguujro.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2offhywbf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2bnksxkev.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zhzdetwa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xodqgxpy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2abydpfzi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ikdnzeyh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2lgysgzji.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2kpheklxx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ddtkcqpy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hjenkzpa.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2wutjbpjy.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xiagufnc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2toxdmwfu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2joybigzc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xufrvwae.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fgydfljm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2zwcxpnyz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zrwxadcg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tddhvezm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ueoadmbn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mfurwrog.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2phuvtpzw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2lskotbgp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2titmjspp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pxunlwrn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2urcbdxxk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mfokaiuc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2iypbgglb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hmikxgih.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bdoqnjwp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yxwqrspv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2azvzlqab.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hlsboshv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2umgtcqsy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2uzdtcusa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2bbhvyian.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jlwxemjz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yzrzvwvp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2aeuiujnn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2fstjnwkh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ytslyewa.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ykiehepi.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2sdlbcaez.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ugfshagh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2joxiazda.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ueqpzvle.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2oymgojzq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2zhkorhtg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mpxsuill.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2efmfptrd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2awjxngei.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfnuddpv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2spgftjud.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lvpiywnc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hqkfskfl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ksofrnbj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2gozivums.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2simoojvy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wabhhcln.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rfijphbw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vvmdfrrm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wmmrteli.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2yotvsmqx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2eqclhola.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2xkkqkfrs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2dmarjukq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2lbqjjkhu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2afvxucjd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2yhefcmur.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2fzhjamsk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ocjbcbcg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lektslca.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nfphbndx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zzcrpcjo.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bfzzyumg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wpxzeamr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2huyfeixq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2jjyeuaou.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2inpcwxnc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2colulrzb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2gqjadrup.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ncxdccpi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vbryauut.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jqrvsncd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2alvjqkgm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2itkxtkvg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wdszbxqk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2dnhozqno.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2omzcgqwo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dhrimaza.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ywbuqysz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2globfklq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2blgopexb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rdbkjfxq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2eomaulei.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2cijufbps.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2sftntrwj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ngjccjlx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ibzghpfa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2suqystva.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ybqzkbzq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2gtcipkcl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2qmtiausk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ykkoedie.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2bqbmslyr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zzbxpcfs.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hhsbkhdw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2pqgazjtz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rvgwpaxl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2utswckbx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2quawkjlh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bvksmgid.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2reuwbqxo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2kmprucrf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2wbcbhoww.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2sytjfgfs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kswtexlr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qubbyqvj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2tvgxchyl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2zpttebyj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2baieeaoz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2bekqvxtp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2uzuzaeka.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ukmipqll.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dvxksldc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gxzbfvbd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2eluzoqzb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2arydqcgy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zmxysjuk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rsyjgdfq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jkzqkvrz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2tjjramuv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2uttcdfql.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tmwtpagc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2bqnbsbrd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2tkkscfmc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2msxvhisa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2bpblbeez.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bbreperd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2nnvsryno.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2xvuwrvtn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xxjgpszb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2dhbcimuz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2auuxcebr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2kfazmbsp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2azbxrabn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2nohzhzsa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2tcczeeqo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2tqncvczm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2rkphbuvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gntuqdjb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2fybzsatp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlipohfo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cjvrkexq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2skdcmzvz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2iimhidho.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xwbtjbqf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2impvqlhg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hbpsmpmi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hxxaehjo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2yztgvvqs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zentlwey.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2suycmuin.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2yabemwsy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vwhdrtkr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2loncpjvh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2edvpmwsi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2yrntidqu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ylnfntql.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wvmhtojo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vbasfnjf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2nfyvdwhb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ydshdnji.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jzvkqalf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2arygfczq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dodmlvju.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2xrxfszaf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2laluxiaq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2louckjcn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bbooxuap.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2nslczzlr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2lsavjhwg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vdepuuas.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zrekudpe.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fgidifty.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wcqoslnu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2zysdmwxc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hnstudzt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gbrqrsaw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2fzchfwao.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wzcxrojr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2kxmzwhwd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2uftlkqjy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qzfdxwnu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2hhcglrki.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2svgqyvpn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ixfypxal.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2cmyumqja.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yntmfqaa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xhqvfpov.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jdrhhjfs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qwebbifb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ycknbjkz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xkuiuiht.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mtledigf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ykjrxybb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2sgtghxna.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zjhlikin.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2pojklbht.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2irulsjaf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2eufqxlks.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ifpefnjl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ufhuiige.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2szxuxoya.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2octtopix.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hvaqpnwl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2aaukwbfd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2yflrezmc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lajbncxf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2sbxjdseb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2aavdoyfv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wohdbtys.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2odkpioom.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2cblnaipn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2dxxcuzdb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2tfcgskdo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfboyxks.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ybavcbsm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2egqqvyce.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xdkqaxsn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2emfzsbtc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2dlrmasqm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2tcgsmvms.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2leqeckln.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cvejlqmc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2dkbveayc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2dmjbgrvt.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ruxhavqs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bekxzjbd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2byiwurog.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zojqvfms.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vkuzjpeg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2fxcolvfa.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2mvjqsfqs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gixbpmff.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2vspkkksd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2pfycexln.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2zfljssdn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2errtyzbk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tbtijuki.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2kujkjydo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zjhqxwkf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ockaddep.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bjuuqzop.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2yeucqdml.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lixqxukz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ojlcmqrt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2oesboton.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xxqnrqcq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kyoexcqc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2lncsater.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2fuhkbhro.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2cppmxqgw.html


<!-- 参考信息 -->