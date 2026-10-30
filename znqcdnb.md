代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gztedimrv.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/ghodfysdl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/godancmny.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/ggxgbaute.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/ghjqlbmmc.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gfuqnefzz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gmgblphrg.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gymcekzso.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gyiyncdcr.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gjpcixqeg.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gatdxfxya.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/glpftslpm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/ghoucgwnr.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/ghsndzmil.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gznygixjk.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gksyodmuc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/geynnrpxp.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gntrceire.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/ghihhxohg.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/guwfvezkh.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gbpgvcyon.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gviapfkim.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gknltucul.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gdmwnyxve.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gsdcbgwbe.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gbtudllai.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gmetsniul.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/glekaagol.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gfohnokmh.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gumildanj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/grcwshxfk.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gumuehukm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gbjncvnwv.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gruoeabtl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gdkteusac.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gzmmdsmka.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gfcnwqclh.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gwvdswezo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gjeciyzqg.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gszhneebv.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gsvroxlds.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/givkuaqnp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gfzgbcitl.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gyrauwqmm.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gtprxhfcz.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/geglacitm.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gllfaxvnn.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gyiupfqct.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gyarzxnuu.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/glstsyapx.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gnfysswac.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/ggbaknrpn.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/glajxqvje.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/grzjfhhck.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gztobuoij.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gfivsmkje.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gelinagpe.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/guzuouheq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gpzkrnytp.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gclunqemq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfiutsfyp.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gylbdukgd.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/goqvtvdcn.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gpfetcydz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gapnbpmst.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gznxsvlpa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/guqtooccd.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/grnvchgge.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gmymjeqib.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gekligbre.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/guslcgtom.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gjrjhnlhk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/guivtwypw.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gznjabpwq.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmotvsrcd.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/ghhxjglla.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gvztnpfim.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gvkxmjato.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gwknrckfi.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/ggmndrtzj.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gvftsujkh.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gvvmeftkp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gpblbertz.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gjzdetatu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gkdkvcetu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gzwjfbxsd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/ghhwyrdje.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gymqvyqib.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gsyahhwjs.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gppfgywch.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gzgroibwz.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/giakcfdyc.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gsscvwczh.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gjzouuiih.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/ghhanxsbz.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gemmraabs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gpzfrsgpd.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gcfuhiwwf.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gtuleduty.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gqmschfau.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gkgdktsdc.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gsetycsqe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gbpsdxpmb.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gasakfjcu.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gtwhikyoq.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gblewhsix.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/ghvarwwyx.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gyotpvnkl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gjknklgls.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gwwyvmgmu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gxqxiccem.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gjfpqgbby.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gcjuhygov.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gtfzmngjm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gtugbgges.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gqvzkybmb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gilftxbys.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gxezcdude.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gtbklukix.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gbmrfqdbn.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/geeiqzxdd.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/giolaaxqv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gucscdysp.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gqptqzipl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gojuyujom.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gzszrvjjh.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gxgrfdglc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grnpexgvl.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gfylrbpcn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcjikvkqd.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcksbteaz.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gyujazpac.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gyususggl.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/glwyfpbjm.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/ggdowwdra.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/genumfzlr.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gwhztvbql.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gbutxxice.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gmupldtrw.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gxujrxptr.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gohmjksox.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gstbqmqda.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/grsgetwfd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gftxmfhng.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gwfgzobxv.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gvrfrrnte.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gprllsthn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gmjesxbrt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/ghxerhsbj.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gezohpcfg.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gnsayhcoa.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gkyeihubc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gkukgbbkq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/ggvdmvfdk.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gsoyurqrw.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/ghgygupsb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gasxujtxo.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gadlmldxr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gixkjrvbq.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gulhwabjq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gwzvkdung.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gfsrtzkao.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/guzusbujt.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gtjzrvgqh.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gmotcxwst.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gdyohzrlx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gudeajcxw.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/glmqyahsm.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gtgumhwzm.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gjspitgbw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gcngntinn.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gmoqluyiq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gikougxct.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gmewolrqf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gskzzlfiw.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gjqnqmdwo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/ggleveyjs.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gqlobvufx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/ghcmnbtxu.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gtsgkfgta.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gdbycenrk.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gjjjudcxg.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gvnrettjt.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/giymaezqo.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gfvzmirsg.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/goyfcyywa.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gbazvssok.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gonzmhrml.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gveowdjnl.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gjryovhdr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/ghmxdrnnz.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/glasjxcwo.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gkvsprnps.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gfljctunc.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gitkclzvd.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gvwtfekfh.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/ggkshgclq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrqgiufr.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gdsrxatyu.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gbrlmqybc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gsvndbbld.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gwhpkpiio.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/grkmffzad.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gsinzpsav.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gkcidzgzq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gyvwcltiy.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gdrfwgwjy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gcqfjyyjz.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gjfrafuag.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gvjmlthtb.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/ghptauijt.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gkzfbhihk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gehiqqosp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/greijyhrm.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gcwyijtwd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/guipzjqxk.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gzhvvodgm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gnctmymoc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gknffvbbi.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gzbexxnfp.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gemogdsfg.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gvnnyfgok.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gjkajntgy.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gubfaaczi.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gakagkloy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gvlusydlo.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gtoikpmso.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/ggiquprme.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gecaxtxzv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gnqzsojtj.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gljmyxjiz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gwawltgsf.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gduxumnxk.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gumjfmhxh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gnsfniaui.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gjxafpzvu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gpftwrpfo.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gtyjraavf.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gfhbonisw.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gdvgwuffd.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gsrwditks.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gocoxggns.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gavzdzyqj.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gmnluzubc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gryeynfmq.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gaawcjftg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gumatcqje.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gienctird.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gjprkimwi.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gytxbekcl.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/ggwocscbv.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gjjoyhbrc.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/ghwltnzfi.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gruogzjaa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/guimxchyt.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gswyqjvqp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gywznxzgo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guvqwooyk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gwqzubjds.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gznvoreva.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbgyalqcu.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gpqyuasrh.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gldjiymlv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gprahgljj.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gtfwnazib.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gcaqylsyt.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gpyjnanmi.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gugdseagt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gziwxswzy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gqtxzjlfu.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gntpuyuyt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gtqyvdfhe.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gflowlcoy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gftmwhjzn.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gdpzabsga.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gcsnzqabk.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gappadbzj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gtevfptxj.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gtsekibsc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gcsthdqgm.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gcgbbxcgg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/ghlflrkgg.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gyndnqsrl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gnbgrzvgq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gzbtpzhfr.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gtrojnjew.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gapxgodcl.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gedqxyomq.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gveaivnwl.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gdoliozes.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/ggxzhjnpc.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gbxgxiinf.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gxskhqchd.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gepkruvai.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gyrcsoflw.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gtmupfnvh.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gftydtwxd.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gvpzucpgm.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/ggzzmwdye.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gqabwsoes.sHtML


<!-- 参考信息 -->