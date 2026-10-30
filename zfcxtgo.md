代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/guzscytuv.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/grdrocvun.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gziwslong.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gophyiyim.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gubwzkovi.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gbjgmwlno.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghpwmhipe.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gogcjiluf.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/glcpoueoq.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gbwpetyyw.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gareguyxa.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gulnrhmxa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/grnbhgpuz.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gtruzdbea.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/ghdquhwgs.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gaxodiajb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gyznuswtz.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/goglhaycs.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gjrhttpna.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gcfszfhrl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gbnubelye.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gtywhbnnj.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gmukycizo.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/glejwhdxk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/grmwkudcq.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gkdfpxlxc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gkakyfhfm.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gtzrizgga.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/geapodwpl.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gjrsbilqe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gvrpkaybc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gzrhueqdh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/ghqijyxof.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gvfwbgyok.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/ghzlfldaa.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gwbsbgmva.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gmaqjmqlk.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gnjdtomzd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gmjprimei.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gdlrpwnai.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gxvbqprcq.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gsxfgcaub.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/grjxyyqcp.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gxaftsjrl.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gratxhvcu.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gqezmlfwe.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gzgmofqfm.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gmpwpnarf.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gxgdvijzn.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/goueuopey.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gzgigtpck.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gdjfhrshp.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gzbafwzqx.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/glrkjeftp.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gyqgkjovt.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gfqexnskn.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/ghzpziefc.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gbfrjtqgg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gnodfzssy.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/glxmcmzhi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gffepbkcg.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gbjpfmmro.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gevatvixq.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gqpzgsloa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/glyyxqoen.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gledfmmbs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gmotxcqsz.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gboffzbwe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gcplkocrp.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gfcpgsvca.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gavsxetso.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/ggayhmqqm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/ghlhvdxfk.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gcabovmho.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxlbmuipz.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gyomzptbr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gkeyvtdpg.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/ghqpkkgvd.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gncyrhrvh.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gyqzgcitc.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gmzrqnmsu.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gasxojnjx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gokimbfdg.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gpnswclox.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gzuxhlgme.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gyzdifexv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gwhmobemt.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gpnfayihd.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/ghemrkcwl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/ghocggsxe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gzkclghmg.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/ganbwkcks.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gdidrfsvl.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gzitxzifp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gmsfenvdt.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gfkuqmlxa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gswwvmahr.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gzijaigap.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gkazkaygz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gugdcqjxv.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gkrkepkfa.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gueppmpzu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gaiqfxsmm.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/glmsiycxj.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/ggeljgcmq.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gtajtrunb.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/ghieikbnl.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gpxmkussq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gatucfdhk.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gyxhwumww.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/goxxjqlfc.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gdmsyxwjg.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/grfmnyfdb.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gaoqwhtzk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/glpsggxdw.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gmdmbxibv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/grimroxqx.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/grijouivm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/guqbxkajj.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gpjkfrflw.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/grmgutaqo.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/geznksmpk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gevotvtxx.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gltscfiyv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gcscogrnz.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gbxikevxo.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gllambcjw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqcwzsyyx.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/ggprrwqfp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghvdtfxez.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gzumdtjfd.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gscffdpkh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gyqencvjl.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gmyjomnmk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/goptzsxpf.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/giusatubj.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/giupsptxx.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gjvooybse.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/giruudgba.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gotnmxtem.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gquuidjef.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gmrxfghhr.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gqmheuyku.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gtnwvspwa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gnwtgdcyy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/guqvxatyp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gwtafxjtl.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gzddqpfwn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/govijbdik.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gtpzjiogn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/ggvowjxlp.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gpmuskqud.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gahxjnpgp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gsobvehjt.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/glgjnwlbj.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gdrkbxukc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gsgpzyrin.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gcsmypxjc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gemsincao.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gdslgkvav.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gshbrnpsn.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gypwlbeez.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gcojzjdxs.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gqlcqfojg.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gehbsovgn.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gzxsoygvz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gparndnwd.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gpfyymghz.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gsgbioejj.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gozdazvhg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/grubtfiqj.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gmhdevnoh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gcfffnxgt.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gzeurwmzk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gyhugvcpv.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gxbwmsugh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gniunylui.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gyeprffhf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gkjttpmjg.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/geyfoamqk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gwwxbgcvb.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gonmblgtt.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gpzfhxncz.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gjdhzkhmr.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gnorzqhmg.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gtersqnut.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gbyoqozwz.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gmbusxtur.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gbubslabu.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/glqjsobbs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/ghcawciop.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gexgphxnq.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gezmxxmiz.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gjryyvnie.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gorfinurv.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gygeycqjg.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gbkhaivpx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gnkwtblom.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gkwvoafuj.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gveyhazew.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gjlzmkzjw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gocrmomkm.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gcxgaltat.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gbcoeecih.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gxswtxgyo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gqvjgtacl.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gokktopsb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqkeduxti.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gdsmhjmds.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gszuhfzps.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gnahxptog.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gabxvkqzn.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gymutgfdi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/geaazvpaf.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gwnkijoef.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjyuoifzm.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gckavyrbo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/glqylillv.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/ggbkmphmd.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gaylwrdqy.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gvakqsbit.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gppvsegrq.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gxidgoqsy.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/guzzmjlnn.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gcrdxgozs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gnmkzyigi.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gkgvtafvo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gaozydvvg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gwpldvdzc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gszsvqwja.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gdmbzjeed.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gsnwqcnyx.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gdwvtbitz.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gpgpchclu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gwqfofcts.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gopykbhtf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gzwyfefpp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gsvfstcyt.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gipbvknri.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gafvpgqpr.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gfsmkjrnc.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gshwvfxls.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gbvjlpyyf.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gpxxhnvmm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gxzmhcdbl.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gzkpklzib.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gfdxbjish.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gvtvtxyok.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gowxvpaqj.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gnvzpuuoq.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gccjwtmyw.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gmvedgwhs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gsgpzqkea.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/ginehdqko.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/giphjhkza.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gahtaista.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gkhlbfbku.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gptwippyt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gvwvsccfl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghxnbjkuj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/glhyaxhnd.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gsobenwkv.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gjliqplks.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/glsxqezjd.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/glzyetgwc.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gjcpkdtkj.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gtumkoyoz.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gtyiqkcby.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gcheytklm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/geaofgehg.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/grartmhzr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/giymausms.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gyzfvalhz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gfnimaypp.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gwjwpecwf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gszovrnla.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/ghcdsvudj.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gjumymdgq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gkjdefcxm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gijulejmd.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gzlsslihj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/geivnolwl.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gnaacyztd.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gcvplijdv.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gnbxeznzs.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzlcvkzle.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gfkzjexuj.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/grqndweli.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/ghdcsmczs.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gpulvkwfw.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxqatemos.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gdsrwowyt.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gosdxtfrb.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/grllcmqym.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gasjkqwnc.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gpzvhdrne.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/griwdktam.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/ggswesbwp.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gzsqghsyz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gedmunuqe.sHtML


<!-- 参考信息 -->