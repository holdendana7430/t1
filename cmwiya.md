代发 wailian999

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2uamfadwr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uhmzyzfq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lrzasugg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2msszwszd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2vzobnzjd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hnfgsyzk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wavvrtbk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hdrplyej.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2qlgsawtl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fmjrtujs.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2tlptciqr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2bcafzlbv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2epqvszvf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jwicfhxy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xpwedobm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2cpdkzdsf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2lofxzwrx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bafnjndr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cpsftdcl.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2wixdievn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tercdezk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2zcxeuqdl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2sliymxsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2augfclwa.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pofrnbgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dantutky.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xqqkqmgh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cbfasdtl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xfrsokpi.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pdfytqpi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2lvfvmhse.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2rvwzwfba.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hljaxarh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2sjqiunkr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2muvzdnik.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2jueacccl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2bohexbof.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2blqvxhfr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2krtxerwc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2yxynepcm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ygqbvmsi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2uletblsh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2dgvcmyzj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lnljvpxn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2wiigpprv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kxeiezvt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2voucpkzx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yuqxdbdf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2xkdepmrc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2aazdzyjr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hilzfmie.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2lykgoldj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2qxewewcu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2azkgywls.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dblujlxv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gxuwfsye.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nbqxaoju.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2caaamvae.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dimhzcge.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bdygemji.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2sqcuvgmc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mprwafqy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2iygnrmpt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2nwbyfmab.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ycgouvza.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2jfelmecu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cgtqtnku.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uasrelwr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qvmjbvid.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hvhdvxiu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2zolmuadk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cgwzysrm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ijgaljgd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vjolumeb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mmkwohxd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wtkvybkp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2fpajbmqa.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2drgkpiji.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2yobzndhs.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xsuwbsdd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qaaathfx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ttylnfgx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2lyjkgbqo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jikjjsvx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ikcprekp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2lqnlswhq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ugbhuhrr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tvudfqrw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2utbjzqeu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2dfbnuxxl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2gdlaldtb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2msvivkcv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2dprlfkxl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2hxdqwymd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wjeqmvjg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qhesxivw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ogkadgox.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2krboepbk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2blezcoik.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2flgxaeaq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xfsyaoqc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2oiajkuqu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jemjnvyu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qozhxmxx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bziualer.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bzasuwpr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2elxcepoq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2attpztwe.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xpxxdoca.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2xzzigihd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rmqbzfyx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hzquktih.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zqruyeod.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2zelotqid.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2sjmerwpa.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ymsdtwbd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2arrgijhm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2tgbhhimk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ouuixghg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vzjkiyft.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2tmjpxwll.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2dvzwoqki.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jwgvjiku.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2xvfonnpk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qxslwuxz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2tacyfaln.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hayknzyy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2honrrvym.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2efgnhram.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fpvmsuub.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2puwbfgze.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ovlcnrio.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2aqpvoqld.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2dwrwuleu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ckjrldbo.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2waokpxxb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gjsfztta.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jxrjfqeo.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2stbmxtbg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2zplbmydv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2pxtxaevs.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ztfvybow.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2eqbbcmxg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vdfgrmxg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2zrdulevh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xawdvegu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2zciewtaj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2urfoxleh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2wqwkexzj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rshmuwhi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2uwxapchi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2mplnqmrh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dxrskjlw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2lckkqkeg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2djyzgbhw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2kfrlxknm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2rjbsodtw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qaagvqay.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tzvalrxf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2aadhpxjs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xcenbhtf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2axxqgwrn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2obngtzpy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2guoarqzm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2uxtghjvm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wpracuyk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2zpaqjsnt.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2uloqspgx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2soumvcob.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2bmgbqdgn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2mgunefzi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2glkolqlt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2agvdgytg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xafkjxyb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dqqprbqv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ygesvrgj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2luqlpykn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ropbvhum.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2nirukacs.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2kazqfanb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2temsgnif.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2uokkintd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2iibpdkfr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2asuvtegf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2grqttktl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2sjyadkfd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ofqfdvld.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2cdirehrq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2lykylyew.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2imkagzkt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2fyofajrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnoqlnyf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2amsfqgdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uoxgldzl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vbmianhn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2tsbrodig.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2fljhfazv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tmybtnzp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vilgzmlr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bfurjwrt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2oxwpnqzz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ulxuexyw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pkwnpqgw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fuywkcwt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bhworjss.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rfanibxi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2rmabrcqh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lcgrzroe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2zhrrezxk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2pslwtivz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2oqpdvigy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ozzozdmu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zuvekora.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lhzxelym.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ukwhoyjx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2swddoeju.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gzyviiar.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2wentsaub.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kodoxfpe.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ihvctlsx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hxqskvkz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2modcxnlg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2gkppqypd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2cdwjfjpz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2coyiekui.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bodzhevw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2bmidgbix.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2naybymuk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bsnixtzy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mrkeyarg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dezrmeka.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2exxvsneg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lefcnuzm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2eadsrjdw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sgpjnluk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wceqpnpt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mdezodjl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2tvcjqnwf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2utwscviy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fsrzgpdb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2iucestux.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2sjflsnsh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jctejrjx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2uswpxeeg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2cwektdnz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gnioholw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2jxpmffpw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ytosykll.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2pwtzzmxf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2kwlhaeax.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dzbfstlo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2pazvglvx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2aqxfdqpb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2dslpjqol.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2slfnnqhn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2szcqbbjs.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zotpeshz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oxbkemfr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2cieyhcyu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wgslfkiz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2kiwpyjtz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jwdbdrqz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2phhwdxcx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2oqgqgxnj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2kcucyavg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2isqsnbfb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2fqtqoikf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fonzyocz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ajfvusbr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2whxdbowe.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2obmyqlje.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ctlddzrd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qfqjjdln.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qxcuxohh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2hekenhpi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zfcuvuie.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2lmhiyqxu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2knzvidig.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2lxxhfwkp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2hrjyzyrf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sfwnocqg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2reznqbtq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2iwvgknso.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2lxocknqt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2mtvotqdl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2jurvupzq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ctbkreum.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2aodxnnzn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wqvqrgke.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2iecvbycb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ugixofog.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbhdzdwr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jhuwzdjj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2tpxrmmnz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eiwrevyx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2sshrctzi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xdvlqenw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ylipwukb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2thgqymrz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2qousyrwl.html


<!-- 参考信息 -->