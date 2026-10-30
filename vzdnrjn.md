代发 wailian999

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gaorpizah.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gevowbnqi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gszyfxguv.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzkmytak.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtegipghg.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvhhhptx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkdamsfek.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjziyfqbd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyjcfniw.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gfbdzmvpd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ggogifssv.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzmuxkllo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gyckekihf.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gjhrduwgr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ghedfpcxo.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmfpeepp.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gphqvdbnq.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gfsomekey.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdqcblhh.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuvbunlr.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmblksux.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gekqxipmj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gleexjept.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/goisetlwj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grtokzoqt.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/getvnymrc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ganhlwmht.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghjstbnkk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvcaojpr.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbxxgagq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giosgjwpo.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gehacejnz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuiipfxx.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsykqxxpi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/giigafsxy.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gcgpopvxm.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grhjrxxqi.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyumnfuz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzcvvgrst.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoyngpiz.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsdmblkzv.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gbdgtebsq.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghmywlvsm.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grkrmpwdi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfssehkhf.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gsiezgoei.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gmwikhwnt.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gyneidwxd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gohlbvgey.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbivahfp.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrqamity.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/glialuxrk.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/goumnwjhz.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/glqjkcqai.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gjssfkroz.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfitoyjzx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/grexgfuvk.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/goezmhqou.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnehxntuf.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqjqvfga.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcukinrjr.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyagrgnb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gollcdfqp.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpmilgmp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmmxiitv.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gthvqraae.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmcywjtq.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoluottr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gnbcjtdfz.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gqiqnfpbb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gqqbkrfgg.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggnvlhnqi.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grsgfgwok.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcrldvgx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ghipkktcz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkjvxywq.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqnwrsjf.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gvgpkzqdb.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqafxjal.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gykkzxdnf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/ggpwsgdxy.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcgvrfbh.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gaegjlozj.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgygprpn.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlxnsnjy.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrqwdlfl.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gbyviuvvf.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/goyrjhawm.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwcnvmoh.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsjvwmfl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmvlisca.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/glsuhkgtn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gheqkigoy.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gpivmamwq.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpsctmtmv.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdoeqbjr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gdhvrnhpb.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gnqkjakxq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqtsiepmx.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gzadjaxfv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkrdxwaf.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gqvnqpbmh.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gohadvquc.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gbazlrvpv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcshihijc.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdnhecxh.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocfjcdmu.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/guznjacnl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwehyzsy.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttwsevow.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyygtipz.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjazzkyu.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gfatgfppe.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtiegciwd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyxzchpv.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugswhmeb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksxdvuvz.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gyhepbrfu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gawvyleau.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/guxlunayi.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gykbqiyll.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsluhugrj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geranwvoa.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/grhbdjeft.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gontlncsx.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gwdnohgki.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgwppwln.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gdctbwwww.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdytwziz.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/geinbeqoj.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjmydfwp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuyrvhjp.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvjxargn.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/ghjzjmpwg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzreqmhpa.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gzslxgtgb.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gntymgfax.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/grnlfkvej.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gfqbwdtsh.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzzzveoe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydzeywzk.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gqbvsyfls.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdmfyacdf.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrkuugvv.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjqtawgv.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gnbmwnfae.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocuxeotb.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhdcgnmr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjavqtzb.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdobjsyv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsutcyvu.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdnruyxm.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpbxqkhy.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gthiddhrg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcbokoavr.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmicbvwf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnwicndp.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gvvbfsygn.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gidikopxw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvcegxuy.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gzkkccmzf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glrkpxwbv.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnmfjonc.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtiaostt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guuyfwjyr.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gsojwfuef.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gvwwdqrzf.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibvmvdhb.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaktonbqh.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdsyyqlq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvxgtxxo.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gnkfmsjmu.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gnmzlpcsj.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazaalekg.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gfswhshpm.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gppxqkclg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gkthivftx.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzszdzkv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gqrtoufjx.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gguwqzlzq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gfehxuqby.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gvlenfseo.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gygrldniz.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gddemgpkr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuezcrlo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwrncqrs.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/ghuhkbrsl.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gewkprqzc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gamtssnxr.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpclmfrne.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxaberax.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gnpqqyyql.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gkybnqdgo.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gchhprgju.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gkpivtazg.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gbmcqyxcp.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvheghqcn.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpwddqbt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntkoboux.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxixnqtoy.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjpulnew.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwfgonqa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/grnrfpjjc.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gesbdppvb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gqejvobib.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gxfhtuvvi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glegpvgen.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gzddvlkph.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gomrcevzj.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/govqcgoov.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gngcflsbd.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gdnhxgtze.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gjhbiydgw.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvltdvzo.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpffiuphv.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdbirbva.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/grcwyqeaj.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtiexcui.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gyjaxwkkx.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfwwwgzs.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeoxobzi.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grfyhxbrk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmkgmogm.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gapggdyrm.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gczpdokzg.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gvtlxredl.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvebwxhw.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gessgdihv.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gbabrlzyf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gojzqrzci.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gikyxoakq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmpxaqun.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjprjaim.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbolcydl.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gijmdpghe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfxlfdnr.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjacdnpqi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gbzwrueec.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvfsnlfu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gbkunecmf.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzyrwnhh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcphvnhds.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwfbqeto.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjlvvezz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmypeddjj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrjomtef.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/guoipgtvs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxgbmvxz.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcosopkmj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwvabwga.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guoscbuql.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/glqwwxvbx.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gulfasgac.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxxkdvrw.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gzfwfegdy.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/galactyrs.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gnzskcazn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpfxbmnj.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gnivlilxd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmrvdlbp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluxxithq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxznisozd.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqoifqnif.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkpglxdm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoerepry.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqsxvmqo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gxrwkafhu.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/grmaoahxo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gonirfksv.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gfxhgnlwf.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/goezwmkhx.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gahmaehun.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzvqgsmc.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gnulbxawu.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdltyoyvz.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyojqztga.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gkyknqppk.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gnqpkelkm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfwnyyqd.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gfqugkngq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/guwqthvjj.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzczhnagw.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gvqoyvvbp.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gzwwuxaxu.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gtxcmqkgs.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gimwxnuit.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gbztusewm.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxlkgdzs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/giujylryt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grgrcrqsh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmiqkthk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmntofdgq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmkjfinmj.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/glkkvnkgy.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtgxtbhjy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqrrzpka.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbscfyts.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnzbldks.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtkonwfr.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gwjrrepke.sHtML


<!-- 参考信息 -->