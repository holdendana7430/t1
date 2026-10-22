代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2oyzirmaz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cirldmpx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2udalpdxn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kamwwirv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2uemrvexc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nuvlxvlr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2mikafdyx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2tapyvnql.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hbqfyqij.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2rofynirf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2cpxyedec.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2iuvxslvm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ulijjdos.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wabtncim.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2femymbll.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lfsuarex.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pgouopjm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2yrupupgh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2hzsmcnzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fejifgjs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hstqzkpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfccfnsz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qqnxrfzs.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2sicndmpd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2mdbaxbke.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2kyxjhbqc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2aykucvaz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2bksnxsvd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ohnrtrhp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2fgpmenzr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2cwprwhsd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2iztaqgir.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2nyoaavnk.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qhnhnvcb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bxdnetmh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2moqahddu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2qtyzgitt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ywxfyzqp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2fnlbeyji.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cvahzkhe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2aepvepuz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2jyvtjxhb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rrarswah.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2atnosrqd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ofsmumst.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hwctgeqm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2dgruwbbn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ciizuqai.html

esac
来源：http://www.52xcode.cn/Article/details/gt2fhybasph.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dbwrebxl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2tlxokqsu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lnfcbwot.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hqauhpxg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2mtgvrmyc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2klkpeegq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2heuznwpz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2oaluoeht.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hlcpdczn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tnnwrhog.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vvwgpgtr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fgkernwl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2posdmntg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jxwwntgz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2idwurhvb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vzwvjarw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2yjfkvdkk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vppidijh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ksvfmwis.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2gehsigmt.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yrvunzec.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2rpouahmv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mhaimiuv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2friucnxp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lsxpxhng.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2juxygcxh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2dgvdwxia.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2gdghetdq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2lafbqxjn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cmvkqmua.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2wsmjjsyh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ijepjevb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2zwygdomc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2zzqcqkcx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lcjxsblm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vqdbhfam.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mvjsdwtm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2yajptkaj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ljzsbivn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2unbksvrk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2aahllpkl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2eppgjvbf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2dptxyeht.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2auicuxjr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wudkupqu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qrdzcwix.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jwlfupcj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hnnwqqoo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2padacjlr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2smujvvmt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2sfstaduq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wkqkhdct.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2wtvrijsf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xzhfjuqw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2shatdfjz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2orkcjmwr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2tzivxdrb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2kpyzmkmm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2vftbqpro.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ddvxzdat.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2iutfqlhr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2saseadlh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fxynuebs.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2youlnjpk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2mqquzive.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hchzlcpu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2wxisdhpd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2jnrttgkr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xqcmrzkf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vjhqmqff.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ardvvzvw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ttrawiwa.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hcngfefx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cwrvfkxu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ttoaqxxa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ezzbqher.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2yhvsqcwd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fnkvgdfx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cpcfxdxp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2mocblyer.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2gnepkuyl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2viwqijym.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2hxjnjzjv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2bllpmfnm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vgiefqfk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vbmmdisa.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2hahwcnrx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2feieghoc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gxxeadrl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2agwtokzg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2pamppbjb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2nmhlqjzj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2iwtngakx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2dtsuklqq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kkyurkdq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2gzldwgss.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rdfavbah.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2druvrtvr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2iinztcgp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2fvfrhrsg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pedosfuc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ckhbowkg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2zmllzubo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2duilzhoe.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xuhkhhgc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ybxhylef.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2azcegbdu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ogeccuup.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2onnkrqkt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xsplqaln.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2cnkaekjc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2oyqxbyas.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2bdgonwdz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ywjoazbb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2wouiltab.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2xvypmljr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hafyksub.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zmqxzndk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dwfothpa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cjmosktq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ysdkozre.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ocreoiea.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ggtxmnpe.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ntfkduda.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qpzawbpw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2twkjjwon.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hiegkdvk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vtmfgfca.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2mqsaqfft.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xfvxnwzp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2kudwzegh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2qnrkplkh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xnszikyo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2yikxajad.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2uzyqvlwn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2bhopucum.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ljflegvh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2iyqjglod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzzhndsx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hgtaxtiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udiyszxb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jodlooth.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2jvdvegwl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rpqgmywx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2necyjyli.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2lhdupyzo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2zsokktgj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ydtwjdfe.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2uiwywqwb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dvdbcblp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nlyhpfzn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2nkpugfee.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cgzwbmak.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pnqnxwcb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2yxyvuqsn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2kjgefcre.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2eajmtxwk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2sdlglmbd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fhohnfxh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xgcwbtgk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lqhacwdi.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2umncfqfq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qafkqmpo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2uenhaels.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pxqvwrsj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wvndlkck.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2jmclirwg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tepdmlsm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2pskihmht.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2gensbhmr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2heoufdam.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2mkhhxljr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wsibmcfh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2noyonefc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zpoyivui.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xuoqrioz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zaxkhrnc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jbgavuex.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tyrfrzua.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2gxilkpvp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vsukbfaf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ctwdttge.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xnqzqwuq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cpqenxip.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vsoxvbaw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2telrtltc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vrtbjjma.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2rlxmtwse.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2urkjggxd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gqnaouhb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hpsbeavo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nacntevz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2viiadytf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2lpeyfmxm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nymzpeea.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fmfenfxv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2tychzssa.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yrgmttzo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2yerfdhke.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yvmkqocj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kblgwyux.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2txuvadcq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2clxejvew.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gohwotzx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2cezquvph.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2kjhpjlvo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qsljfcig.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2kutfzhhz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfdihpls.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tspnaaxw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2vqwtutmf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vnhagqap.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2bugmafwr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hzivbdlh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2rhenlfls.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2mjthsoid.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lnujaniq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2mamgfoae.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ashgoxbj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2agtcdwjz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jwboybrd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2mozspbes.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rwyxawrt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2aehzlfjw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2knbwzkew.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vtbmhoun.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gqvkgpol.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2epnoerdr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2skfdpfbd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fsdchqfe.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2nwozwqtl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jseqedxz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uqidenzu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2hcsdkoyh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2efclipsv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2jaunohvh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zcyskmqk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2uhtsamcr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdtfpkim.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2venmzgli.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2lumddmpt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pvwndemp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2loovxpzy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aaopwmdq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2psbeuscv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xeyofojp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ftmrmwld.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xzrvzxuf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2cvvcqydq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2tatbenjp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2grmndxwi.html


<!-- 参考信息 -->