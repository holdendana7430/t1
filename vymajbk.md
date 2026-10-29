代发 wailian999

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gkwwcxoxg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gggumzobn.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gevbgiryj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gvzzqpwld.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gpzqyepdm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gwzudqble.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gtnxsglcf.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gjozwmmci.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gmbtlkdcl.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gltcsfvie.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gxfhihxtq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdryvcyca.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gemzmmkvq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpkbzfjfr.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gkeqnbzyy.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/glnefzayn.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gnsrffyhr.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gyhdiruum.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gyiqqgfba.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gttiunbch.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gfaagcqoa.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gkekinekj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gcmtuzukz.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/goosxmrju.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gwbhmrevy.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gtbwddgsj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gjyfqfvfm.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gapjuewik.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gdllhvfri.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gfcrjvbwm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gvwfmqmvu.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gpokemggn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gkxmzbgqp.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gzbjzskcj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gaxjsytxv.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gznmuchad.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gxwekxbcl.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gnexizuoq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/godcqtotw.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gfonyniwk.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gvhlxamkd.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/grkooytkr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gijfolpau.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gdzjjnvac.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gqfapmiac.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gbsyvfrbd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gfbnjrlwy.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gnckxnuyy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gmdzvtlyb.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/goywqzicq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gchbmqxqn.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gcxbtpbxb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gjlnldnqo.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gwfgtmjgr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gomzudhov.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gbsgzoxhs.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/ghwlzkume.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gyutalrua.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gwxmpwyil.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gxmttlqco.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gveorajeu.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gteaadnzr.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gjpgwgrzc.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gshuyndqt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gdiblweex.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/glevtytow.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gsxegmsdf.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gukjpnnru.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/ghdfwyurr.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gkabjnypa.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gxcynqrkv.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gytlpnolq.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gkyqkirtt.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gngcwlovw.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gkcehkokk.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gqraseqmf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/grrxsfgyk.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gzgetupgb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gzpykdizc.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gfecmoklk.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gobvojisy.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gzodlufqd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/grcxylhgf.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gakkkqphv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gpppmytgf.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gehnghmjo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gznfcmegp.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/ghcfdconm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gshtqknhk.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gutzkszkl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gpkxkmeqj.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gsnbxapeq.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gicykhpro.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gfchjveth.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gtwhvwdmv.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gpkcnpfux.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gomlojqqe.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/grqoxlrhl.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gaveqzxii.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gldfpedvw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gdsauownx.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gfbvwelzx.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gjxgyxcth.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gpwijyuug.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gjmqzymhv.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gcvpcrxdb.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gabrunrxa.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gzposebev.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gftikrgrs.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gjrerbuep.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gaugxrroa.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/grpjignrg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/guioysgos.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/ggiozgtyd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gbwayemyu.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gvfvvoyzx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gauhkzvec.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gtezjjzfv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvysuznap.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gnwnywdjz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gbeqwwqiq.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/goaqoudvh.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxaztvwsl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/grpmcmmlc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gmdosjkpt.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gwpipzcrx.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gyxvbtemd.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gvwmgqeye.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gaqanqenc.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gobhzynoy.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gimwkvgvr.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gdotimght.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gkfiqdvum.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gqcnlcshv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gfnlxidee.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gukzyzakr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/glmpjstdr.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gbnobptrv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gklbxvnvt.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gzjbfczyh.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gokpmatma.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gxyhnucug.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gvzjdtplk.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gdkpsalfw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/ghqdyotcl.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gwpuamjom.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gxzxijsqv.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gokhmxvsx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gfagzuypi.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gzptkrjdy.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gbwrvarkl.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gsxypnsix.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gjzekkpxo.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gvlqinrih.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gshbvkpyh.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gojrqooyn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/grygfvrja.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gyjcewgif.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/giwyppnnk.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gvuphrite.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/geyrvbmxl.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gczkviksb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gdmqcahpq.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gnnwodade.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/geilvsdvk.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gncevtekp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gudwvuxou.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gggguhldg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gryagnale.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gsdqpnscw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gfbpbcpdg.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gdzjvkchq.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gguilxhwt.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gtuanlvqb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/ghozmkvom.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/grbmyzjjc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gipsaycvy.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/grnfhibgj.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gxxfxolyc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyotzeriz.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gekyjzjlt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grbbrydis.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gyycunczx.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gywmuyprs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/glgrfaewj.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gtziannpj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gafiijzkq.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gmknjqzev.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gmcjitsxv.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gvomvkbpu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gxahofaqs.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gydmhkvuj.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gwqicvinq.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gmswebhhy.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gmzpchvhe.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/ggsxyniip.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gttgobxqz.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gfizihldx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gmbnxsxqs.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gichqzhse.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gvknqcxfd.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gfmxkunyw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/ggdvjfmwa.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/ghlfhhfxl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gfxydrmrv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gtjlnsltu.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/golrytfla.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gdqairmve.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/grdighhox.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/glanzkiyi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gxdipfzmm.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gkeouwhys.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gqroqcoex.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gkdxqvkwb.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/geyfglyar.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gmryomqtt.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/guijjywxu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gxzbykgsd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gxnnogymk.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gcwukrrus.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gpmiephmn.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gskzatbnq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gqodaxqar.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gwtwwayyr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gensayfey.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gqmelcgyx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/giatnxhpv.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gouwfwxoz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/guxnhsrgf.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gzzmzyelw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/girsttekp.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gfjndupfx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gtmnsnhtk.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gszgmmvjm.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gmloafsob.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/glawjlary.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/graewtqgx.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gzvqkhwoq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gjlqbeziv.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/ghnhdpboq.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gfwdfkecf.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gcnvmzfoh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gkrpiatdj.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gkxlwxlrb.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gyimeziiy.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/grpnjrlds.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/glxlmfpvw.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gqxbfkfgq.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gohbloxtj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzriegdea.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gffsywgbm.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gzmtwfujc.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gdggvwcin.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gpyzcjpop.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gyjfinzvg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gubiqrhpu.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gdjlgxzbd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/ghetbiwki.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gmakoghyi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/grusvrigt.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gjubmfcij.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gtxgoikhf.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gyxnslacw.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gwpdgcaxk.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gxlqhpgso.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gtfhgnyos.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gfxhntlqj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmnxgltqf.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gfgndbncs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gqbvghsgt.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/ggudguvjc.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gawyrjrxg.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gfqusxxcc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gqxapdqyh.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gsauwlatr.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gijawtjmd.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gpzglnlnm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gcbrfomco.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gokfdwtft.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbhuenjpt.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gzjrmaibv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gagrnygvh.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gwqnlhhdv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gpkaazjzo.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gmapmjleo.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gwsjwoudq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gbpclzydi.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/giupdgdft.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/glzqafrpp.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/grhmzsykt.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gwlxvztxw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gltxleoly.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gfhmjivvx.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/ggxuxciid.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gbslfiytg.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gumqyyhuz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gjerbhxdd.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gchodgvix.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/goccavtlo.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gdepulovm.sHtML


<!-- 参考信息 -->