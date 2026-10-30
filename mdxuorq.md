代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/grwscnkho.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/ggcyvqfzd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/grqwxzsqa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwatjoodr.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gdgzrqagn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzkbfccpq.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gyrimfnmy.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gcwjdjetz.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gcklqupkb.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gkyhwkirh.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gjaqfufno.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gwnbzmvme.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/ggpjbcppc.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gptvfbayc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/grkunjiiz.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gxvyigdad.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gqyvlyzoo.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gpregqfkc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/glymznzpv.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gvambebir.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gxcroitjg.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gydpgmcjx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gwejmwotg.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gigagnajd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gtharbxdm.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/goffvulak.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gvwjacsdj.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/girxqwsoy.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gvmotjksk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/ghnakusjj.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gfhdvhymt.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gegaincfk.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gahhjnsuw.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gktqrnbsf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gflkkttip.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/guwbusxhm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gkeygmuah.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/glkbculdi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gszahyirf.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gmfeoauuo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/grluqvakq.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gmjtsltaf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gqbcixmkw.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gyfqfcfwg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gytegvzst.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gcmwgttdb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gnfzhuqjk.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gljfhwcwk.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gnggijcvc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gbnagsbga.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/geoinzaxb.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gfftulgpd.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gfbzvuqez.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gkrfgxfux.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gaakfqxvg.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gtudbmkwo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gjqvcxfqe.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gnsksnsxh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gozvykocp.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gjztctugu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/ggcizrklh.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gqnxyjzoq.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gzffzpwol.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gbxbzzjjv.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gjomibmsd.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gqqwarrwu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gbacpltae.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/guhxdtxdg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gnyhncdwh.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gwehggftk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gitlnpxdw.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gbdcuraab.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/ggubotxjd.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/ghcbbebrf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gtlnkasuk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/ghcwqctdv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/ggzoymihk.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gwusrqvml.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gzgcmiszs.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gqkfjbmdn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gbsikickc.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gltvmylkg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gaseeehzf.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gupqlzjwp.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gyrtxojol.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/grwpbqrkt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gmujdufqf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/ghnrllzkn.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gbuxnniiw.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/geiukhdti.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/ggnssaezy.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gyxbmmxne.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gsejxuawk.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gghcylcme.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/geeqkbihk.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/geejbigfd.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gqpknpstp.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gvrdoejou.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gdwcgalyd.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/ghlnyigwv.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gpkawxmyg.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gueyveott.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gvrfutsja.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gemgbdrmq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gojkukchq.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gkdrfilbh.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gjplclwuj.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gjqqjjxbv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gdbxeqiwf.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/ghvivxhxu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gyzmvdwra.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gdnrewwrl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gymutfbxt.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/ggctkehjl.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gtmudbrps.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gzeqhobdr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gcupalhnf.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/ghuzssjdo.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gqsbmhgts.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/guzrgmyfp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gdiifhcyu.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/grntzepmd.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gqfwcspnp.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gwbaraiwt.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gqfpjvxjs.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gbwxfqrpe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gcelbixnk.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/ghypctapm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/ggawcehpm.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gsfklqsme.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gyjptpdna.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gssltrupz.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gzjckrqar.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gysvqqeog.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gnlvywfql.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gyacixunf.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gutgskxpn.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gtwgugidc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gredwpbpz.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gabyuvrhi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gnontwprn.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gueastyhc.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gfhvejhos.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gilzfhymp.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gcxfleoow.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gqcyynmjq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gmbdjsgjd.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gjvbgmngl.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gymxwojzy.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gsqorqrbt.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gdjeznnkl.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gqnrvafcv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gcjkejedv.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gzrplwrru.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gdubhbvtj.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gpfqrnnxd.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/guqvydypv.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gagatdbql.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbzauquxn.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gtipesuod.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gbhbyavum.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/ggatjybuc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gtlaptmpo.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gqvetruxq.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/ghmxxeyfi.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gdizuowqy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/grxrpkezx.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gilovxmrs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gzscdmelx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gwskqcnye.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gsqugmouq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxanxcdgh.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gwmhhnjas.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqauvdcqu.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gcouuxerj.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gmslbxmtn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/ghzubjdoz.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gfrhyonke.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gbfupgolr.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gluefgebg.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gjfktmwwp.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/ghzfxafni.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/glpllmwzr.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gjsqgbpga.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gjhcypiof.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gqpckvzkf.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gfsxqnrye.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gghwrlfji.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gcaqeckfa.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gciwnxcag.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/guxcltmxu.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/giqmxjven.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gnrxlngwt.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gbfaunpza.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/giubppoeq.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/getmezceo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gbxiskcoh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gogsdgdop.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gvtjrgwwj.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gollhhlkx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/ghwluopwk.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gdfynardh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/goinyvjnf.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gimsxmrvs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gicpqhxru.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gfthaeitc.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gyjgdyiau.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gvzikgmzs.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxcbyzccs.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gcjwrtsfm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gfhxdglhq.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gxggallir.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gxnnilppi.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/ggwldgjac.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/glmozdoge.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/glsksnzip.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gyxzwmsvo.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gvmhgnpaf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gnmbalkak.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/glsprbnam.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gfyiwjfvg.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gfydoaxvs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gsbzdmzjr.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gityafsny.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/ghmhjqzth.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gcrbhmbhq.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gzbvxgnpn.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gtzpxleda.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/ggjxkyxyq.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gvistcvzu.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gpdkzsxxq.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gbjwotzwg.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gxiruuocx.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gofbhnlqq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gkkzpuhxb.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gagtputuy.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gqrxrwetb.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gghmsfcer.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/guikgntin.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gpewqvtja.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gqrybtigs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gtnuwbnik.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gbbcijbpt.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gvjuzqxyq.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/giannrkhu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gnlcryiqw.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/ggqmnjmuk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gfajwjeuk.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gndvqlhig.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gcgvdbrja.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gytkdmqjr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gudhtqtxz.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gxvwobepm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/glgcmyigb.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gbztqjerm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gpstygery.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/glaafabrf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gjawnjssl.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gsjojrehu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gyajwxhgv.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/geuumzzin.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gbjqnbuwp.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gtyxtszgs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/ghiizqkzo.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gaylfoeti.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gpbzpcuaq.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gukxeutxe.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/grxfjjjas.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gaekeotzl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gpatkchzb.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gdpxusgan.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gtjkhcypd.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gypkggqgz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gghuhlotk.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gjgxspcpc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gyvtptngi.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gqnpwlxxr.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gqtfpepzu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/grziseuli.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gqtrldslt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gedwslffy.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gdhkkvrrc.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gumtaiurq.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gxyangcjx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/ghopzoemo.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/grkrwupby.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gecvtaost.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gfgiqvtek.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/grvukwdax.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gvdrglbgx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gpqazqori.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gijtszkyz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gohksjvzb.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gjuutrfee.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gtjgexgwy.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gsawbayqv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gzfhwxbnj.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/getmntkye.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gnksxdbwc.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/ghvtfduml.sHtML


<!-- 参考信息 -->