代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3feokpyby.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3sqplhqwm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3aobxovkn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3hfwxrlna.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3hzyewmds.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ylkubgnq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ihzeedek.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lwfuzibv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3uavganxo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3moxoppwq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3uwltvmdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atbmnlfg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3axnskygd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcclchpz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3irnvyhyv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ecbsniib.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3joueblvq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rgmlwynw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3rschyyyy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ihzcumzf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wkcoofoc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3gdimkqne.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3upowjqhn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nxxnwveq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3vzmrbekg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3teaxmtbe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvqqdtps.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3iukjxanf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3obroputy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3danyqtpn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qyslgmii.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vxbrkpif.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tjxxcali.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wkvdsmrh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vqhsqphr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xzqhcthc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3alptudsf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lnetnwys.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xcvrbhgr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3wkxyrngj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3gvlrtppa.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3virqmmut.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dasaqlar.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kggpvpyi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qycldtdu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3woxepiyr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jnjrbgqq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cmkzydtl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3tmuqzkwx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3zbxtyjpp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gwmxfnjw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3gfptmdyh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3kvxwfttx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rjlirlll.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kjmuflot.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lypvigxw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3rhbuslwu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jahgnldr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mdgsqiwq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zdebshiu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ulvmhtac.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qrvsljst.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3hflkstyj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qlekfgur.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3whskdyhi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xmfcztzm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hrhuzpiu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3cvmxsird.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3mtoccefs.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3kaooolsp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3lsgncdsm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3owyrwgic.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gtdvndvl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3cbxzgcxt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3oxydeyrn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dlvfzwrx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3azousfwp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jldpvqpx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3uzvinmss.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fnqscqie.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hefwoolp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3fgincyrm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uikturpp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3roavkuxe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3domkhzfu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xrsgdrwv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fcnjdavj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3xinpncgv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3voypyfwt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3wwarrlmq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3yeovodjy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3intfovjw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3uhjywoul.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qctmuljw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3lktahmjm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3fmaozqfh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3snhtduch.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3cixopnbe.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3jvnwcpwu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3bnroyykm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cyughaam.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3grognyea.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3xojxjyid.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3lbpegusf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3aqwijdyb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3rlszdlfu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3dikwsemf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3adubcvtx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3iroakykr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hsvulcoy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3upyizall.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3vxbxmzni.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3srpqzgpg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ushyhbwf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3imiwtiar.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3tcdwztfv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3drsktfbj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3xwwauklq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hajjaomp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lbwooahc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3hwnysvsk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3cfzljujn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3caqisesv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3juvfovkv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3aypiiset.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vclvxvmf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3chomecek.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gmrewoty.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3izsculpc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3lklyqepa.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tkptunlf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3sfbwmwpa.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3nnuzcguc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3gvlmyzmk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3jcldiuhe.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cqzoqzty.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hawraktd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dokihvll.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3wtchscda.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3yqzzifga.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3aycywjbe.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3argmpwex.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xcdtaxwh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xyrbmbgp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3mzjngwhv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3onmypkpb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3spvbtckq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zlgwmrlj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mxphmhlw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mztfszjo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3zrgtpngb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3yzxoxgii.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ezlpxkjl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wbaqveon.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3wgzyixlf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3phxzubfj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3jrrnrblj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ysdoldun.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mtkrbuwq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hvagvoge.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ttsptyap.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3yqcnvrdv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kbbvtgge.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fahjlcna.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3lydqldzf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3yfljjajg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ozwlocrm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ifndkfwz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gexddjyy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xblvrclf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hyweawam.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3kbijiyfk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3iocxkpol.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ibdjsyeo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bbidhkli.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3pryujwqu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3drmcfarm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jtfiwtav.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3qepvapgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btlivgpu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3spqjwpia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddlokpxi.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ftnqtbhb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bjbjfsec.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqohdtdz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3eeytepdw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3enwauahz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3dempcluk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3btjtnbxq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3nzupxxvk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zzjnbmqc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3arooqhar.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3duhgxgfe.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cwvpvuvk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3sotgmnit.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mfbmxrpf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jahwrdxr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wtxktyni.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3oojxkctq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3fugatsyg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3flfnbtmb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pzgpmtwu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3aglebnnt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nqtgvduo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ezxgfmop.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yhmvipbe.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jiuapyaw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3knrnkyft.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jawrhpii.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3lzyvgipv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3sxhoqsuy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3dgbwyfeo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3hzdexxfr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ecpcqlzq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3okaalpix.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3lnwvmcql.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mikevktr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vutsomdp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3taljysap.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3teqihmth.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3cimnauij.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3yybbgvzn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qestxjkf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3xyahtytg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3brhmlggm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ewbtydmc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zzpcbwha.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dcvujidw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ktyetotu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mymurgbg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3kpwqrrrr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3kvptvpsa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dvvxzyio.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mchukszi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xegdazgb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xyixjmmb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3wjqjaqab.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3sfstmbks.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ncunyqex.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zmkitcar.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pnbjjvks.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zjtpmroa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pjuipijo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dfdqkyri.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ulbclhqm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jnkavmvx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3pvhsjtqr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cvoprcel.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ldoozhia.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxzpxcbh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3onfqafvv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3uamrmcyu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3lizuezfb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3athyoavg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3haqqiofv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3obyxeaan.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3awjdgqyi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dqxyjixn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3yoltidpf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dvxeiwoe.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tsqmjphd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vcexdblx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3enayvldi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wllgbfoj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ohpgwpyy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vndcrvsq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3utwpozgi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bwtwwvxg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dpwifnss.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3oorpxuff.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3hjomasje.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3usawjron.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3diynyhmy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ujrvvxuj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rupwjldj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3igzlyrxn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dihkqsth.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3kkmdahrh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3tlgctyua.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3uepcfytr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zwntrdbe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycqpkncs.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dseuallf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bcjbaays.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jxnurssh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3okjgyhar.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3zyufqovt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3aobkbskt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3agsbrocd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gpkixjjp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3aphwrigs.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zferkyhs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqmssfdt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3bryffire.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hghfzqux.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3fzvszanz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3pwynmchz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ssqtjyur.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zmjtzomt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wkicdwmc.html


<!-- 参考信息 -->