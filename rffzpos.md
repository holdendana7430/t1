代发 wailian999

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfemcmvx.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsltreiwt.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glytssvti.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gftdfljxq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gkwxirmhg.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimpnfkvz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlovibuu.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gxsnkidev.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggexbrbth.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyiygaou.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gntnmanmb.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnfqrlay.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gabpfvzie.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gmbiygbft.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqvgilqr.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkzotndil.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gblmceqpo.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gfgnqzdnl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsmwmonz.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsctpkuqq.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/giuiixmtn.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxqdrudr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjhvadbe.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gtjqqwtzk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrubtbru.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzaxwhiz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeiseyad.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gddpjqvsa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gengdlmwr.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfcxdvak.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiopymhd.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwvmgfida.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gzjinujqd.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gzovkpdtj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/geaksisja.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcxamigy.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gdntcbzzn.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gmetreeaf.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gabrbwkbu.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gsahfqeoo.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gmywqtstj.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmzifjyr.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkqglkds.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/geduqynnh.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gdntmdtdb.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gverscerr.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gtydkqvcx.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gykieotva.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gmuwyrcwf.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gozdjagxl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gzlhdqxqf.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvetlnxcl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsilhbzw.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gjjttoujh.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/greqbhrzk.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqmygnnl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaulzqcj.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/grdocrrpy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfcqreqqo.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuynivrj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmfbhvrv.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/grjcexpli.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjjsyexu.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyzckncy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczflcwba.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehoynxkd.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/guewzifol.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbwhmfcw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcfuuweg.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpvvzdnd.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gquoretrj.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqutexoz.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gjnsegbcw.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsukswlgc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/glydtcccb.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmbdygrz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhsglwbn.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/geuonqayr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gzkxwhyrs.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gpropsiqo.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjbvldbr.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqbgfjsea.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gnceraynm.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/geevmvvmg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaygblgd.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gecdpjrqo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gozfwvrwt.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/ghiwphcog.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/ghocsdiwh.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrbuuzyo.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmwljccv.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gwamqqpmr.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gebaguamg.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/guqlxncji.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gujpbdzqo.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gftzasswh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gnccvzmzp.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvxxdpyn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmvzroyp.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxpzeqma.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/ggdorasli.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/grdiaulnq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjkavxscz.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gxrdalkma.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjknxwsv.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/glrqotleq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpunmgcy.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glauvvnhm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gwribwruz.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtuldxsi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkgekxcq.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gqzojojgq.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gxawbyflm.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjxggtce.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwtlrhpb.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gemqteoau.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsksvfwla.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gmkzrmkze.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gzvyyekkc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjziawowm.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gkemztaoy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzymgced.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfotsxwse.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjafhzrl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlcgxxpq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffxxunmz.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gjwrdfueg.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynjptgeu.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoukgorp.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxannrrw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgerujud.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/glarjwdde.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/glgsqzvja.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqucwikf.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/ghqsxtbhx.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gqiosnfsf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcjpwqte.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmqezysd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gdyasncvm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbvfvclo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gtezvqadh.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gbefefuzt.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gjsmzdjuw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpgpfcyz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaygtlqk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmxbrdyz.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbtnrghp.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzesezvfg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvhepojv.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gtkyjijvx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gydflpfzt.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gzboengmp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjkveonm.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gjwofsljn.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbwghpvt.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gkndckdox.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuxtiwlv.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbbnrcayw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjujzgvge.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkxuieyv.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gxvokjrqk.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncxgzjhw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/glczcojgx.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gfzfudpsz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gixvquedy.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbzqizqd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gqfgpzvrp.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/glbjorkfq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwgxjovj.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/ggxddfdep.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gylndsnaz.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gyybrtphe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gydnmfmoi.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrrfuanc.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gssuqvwhd.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gwqtffltj.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gvoaqmvfq.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/grufsdgbf.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfavwkqf.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqxerynq.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/glxloxlnl.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gibkygmuw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxszllell.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsejsadm.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gudybdxto.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gywugllhb.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gywcengqr.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnailqzno.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gasatljvu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtshxwidg.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwjprpar.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmhsmzbi.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gxigqfdjw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghukwdvdx.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpsxxdqj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gshvxtdgl.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gcgdrlyni.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaxlylhb.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gyghcalps.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gzpvcabwj.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkybojhl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjvcjeea.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupzsqxqd.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/ggfwpvqqa.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gjivhqtfz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbfyhamz.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyasilbl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ggtpchsex.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gilapsrib.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gejtbfupq.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyzuamik.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gggosrurn.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gigxbzbtp.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gqvqqulpz.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gbhgfqeww.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guhsamhlo.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkblceep.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacjjtkxe.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/ggajvrvtv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkomjbqck.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrkgulyq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcelwtmhb.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqfjuqtw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gplccagzn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gslsvvwgr.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfooahos.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gxcoqsdll.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/ggkwsjluz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gfqjftfmp.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gcqxeqbyz.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzdqcsod.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxhopxcv.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gllylykfe.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gwxgeupul.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/grsvjiyrh.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gdcsulfyt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/ggvybntsg.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpcwyutx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gcxpxfoyd.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gplpfxjhu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgmilcet.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gekdnvcrk.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/goujwotzx.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgqtjayl.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/giawpkyhd.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasmalpdf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/guwtojkct.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gheylphya.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrokvrbn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhjwrnmh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbcqtcyh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwesgmujd.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gauwnejvn.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdwcspwd.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzljhzqzr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gspighbfp.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gwnemjylc.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyffrhzc.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gzamwqhpf.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gqcttiwmk.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/guiuvfvyf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gptmbrjij.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grufhgjbp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gxevhlsta.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxufwuxs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwytonjvv.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gcrdfpbbr.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/ggzdhbivv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwkaqyvd.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gepdzjpwf.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gddrtcfkm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqweinoib.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gqortsqjq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/govztpgje.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/groqneorg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitujexqz.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gokjlkkzr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkstzijao.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gfsvzlyqw.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/grfholtuu.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gtucezimm.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkigltyoc.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grbqwadab.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtfimnqh.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/grbzpiabn.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdauliras.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/ghnimwdck.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gymmppfyz.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gtbgxjnbe.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gjvkomszz.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/guzqvgodk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gigljwxvq.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfoxbkws.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmgfhtxi.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gojtfepyw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmwrmybn.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzxmasxgd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gsysbbwbd.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzlnymqu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfvphjxg.sHtML


<!-- 参考信息 -->