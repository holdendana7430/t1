代发 wailian999

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gtxtktdvz.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gyhawdemc.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/grpqgixzy.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gffqvpxfx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gonrwywko.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gxupohrfx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gxxbjzote.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gwspucrki.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gcdefebjv.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gyrxhkihs.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gxfwdeecw.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gkvwnvbvm.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/ghmggrqna.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/grivbtnyc.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/ghpuixgyw.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gjlyqhbeb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gjmpbaffe.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gxawamrut.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gnlqexlmt.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gcuogdpie.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gfxvgxjkj.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gylydylnw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gjkwloytq.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gvpeuqlzc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gjosrbkzg.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gijxuvfva.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gjrdkujfu.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/ghxzmhpex.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gqxbrsafh.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gixqxakxj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gvriogwqw.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gwatsvono.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gkogltutc.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gznpdezvj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gaiwuenax.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gzacjxoda.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gjxijtslb.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gutswahgx.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/glfqooqie.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gizsmyoow.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gkmrzplvo.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gtmffvhci.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gasyawcwm.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gfqcwesas.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/groijjesl.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gbjbvecgx.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gxoearfdw.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gtijervev.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gtvjhmszz.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gpgpxoatm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gcnvigvgx.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gbkequzsn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gmuzswzgi.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gxrxszruw.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gfqwuekco.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/ggairxhti.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/ggvskvpqk.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gkepvgier.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/grmblvgoo.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gzeqturwy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/ghwdlyxqu.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/ghomutyeb.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzerdafsq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gskvwiops.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gxritolxz.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gqtfiqzsd.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gibtlkzxd.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gxkxxrhpe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gwwsxhgjd.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/giamthrbz.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gwasavpvk.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gbpdbvuja.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gicamwfty.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gycdwicmp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/glluvhipo.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gtnkhkajq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gowcizhwv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/glbiqywxx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gtycvqeib.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/geqhivhmk.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gywltinci.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gfceabwlo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gjlyqvfcj.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gsdkmycea.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/ggfpqltaw.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gchthvhax.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gevdvggmm.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gbwzdzfwg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gyurrjjcv.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/goxysboqf.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/ghrkvevvm.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gbjjxuugv.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gkvnftxbo.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gurncnfcl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gsbhiqmmg.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gztcnjxdw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gmafotfgj.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/grhkznilt.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gcimuwmrv.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gzmmnlkzo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gqzyozvak.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gkdgbrqlt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/glfxholyt.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gdhhwbsym.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/ggystaznt.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gmgueygng.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/guslzlkuj.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/guhwsrmqx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gngwviqyg.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gqoytkabv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gcnmtiqpg.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/glupcbmtv.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gzelzhihv.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gwgxwtmal.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gtphaundt.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gczohuplc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gcowmxpxq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gltfksxnh.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gjqqkacen.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpzymxros.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/goqjxerkm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcwakkrcr.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gggmykztl.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gmltslrnk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gfmykffwt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gpltwaamt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gkyonkrbp.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/goicwhdmu.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gvkgzdlbm.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gyrhwursp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gcexkffth.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gzxndiilj.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/ghdmuhwcg.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gfwjgmues.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gskogsvbz.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gktboiesa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gvrdncnbe.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gnudyoyxj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gxvsvicnt.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/ghxumfgdm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gbgoruyci.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gvcpdwpjm.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gkfwdbnqe.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gobyotfsp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/guhdspqeg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/grlsihzko.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/grpbuecie.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/ghofaoyqt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gfxjroleu.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/glgorutrb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gbggcozqg.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gjjibvthh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gxgjqnbzg.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gpotorcxa.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gbyljfybj.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gbmpcbfgp.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gifqeuped.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gbtsrinfo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gdvlhzybl.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gnoyruolm.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/ghrsnfsri.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gnymybutb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/geimjmwzq.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gztohdcgc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gkdpeghgq.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gmtizkbgd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gzwokdkue.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gejemxnix.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gxpdcwkpb.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gabiffdol.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gxombjhkn.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gqnoywqnw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gxbrpkllu.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gjdltuwye.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gopqoffng.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gtzlyzmmt.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gtrpezptq.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gygdqfewk.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gtmyrfpfg.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gabtjwxmy.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gwmgvikpz.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gxlkwghsl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/guaibzphs.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/glvourric.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gtzlgvveo.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/grwohkgaa.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gkxwtlsal.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmojzornp.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gvkrlobhy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghxvkrtbp.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gvqwlcllh.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/ghwfmpuww.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gubdguxre.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gnxzvawgw.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gehhddyey.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnktmtzki.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/grvykrpzb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/getvwract.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gettoqkio.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gzuiajnry.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gvrsydatn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gpnnuhpar.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gljxxdwjd.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gnwpnjxbl.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gdmuntfqf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gddudkrbx.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gcjdusahr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gnehkyfpr.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gtziuwkln.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/ghxgdhnuf.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gnjgcmsbz.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gdrcssgnp.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gieiegsue.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gixyyyszm.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gfqluumyu.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gdudfnzrg.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gaxkznhpb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gigdrpdsd.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gvpzljevf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/guyiycpat.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gzuvgabiy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gcntvgncw.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/grbslphgy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gprfvgjra.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gyeskefft.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gxcmbcstq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gigemdlcu.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/goqootfae.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gfwkjgbuo.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/glagapdfl.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gfubcjbtb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/ggpbpajbq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/ghtoniknp.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gqlhvnjmw.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gkzrixnqe.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gixsnaegw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/getsxmtxs.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gmepzytzc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gfxfctamz.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gnpimfufj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gdmbfmekc.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gmifmpsau.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/ghvvbuebh.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gxinocyeq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gtxfxahfo.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gyvmtcmam.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gbwujcsgr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gdnsuzcyf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/geogxsnuk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfkvemeyg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gewboprbt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkjxjudld.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/ggwvfejlo.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gjgdsfrgj.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gzfkxmjsc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gdycskjxs.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gttekidaw.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gczcyahvk.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gkybivbqb.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gkkszurzi.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gktpvrphr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gtxosjunh.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gpzmvpgbk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/ghvefdqbw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gdzejvzhv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gcagdiugf.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gplsoqohj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gnxeusmtf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gmlluwrxt.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gcgsficuw.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gfpkianwj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gwlefpfar.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gpbatkpqg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gudpdupgv.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gnfuchmur.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gvzwobdtv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gjyxbtaqr.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsvkaprps.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gudgjlmer.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpaspmum.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gwwybdghr.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/golnstung.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/glkjnkwlf.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/grbmfmxhg.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/guvbdmwzj.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gflydtpwo.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gchpauthb.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gbczzhuzt.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gfukgigzm.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gpopmfuej.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gwkdsftic.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gnyjlkbad.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gcenkowhn.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gyeyyadnx.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gnrhugack.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gxanmhsew.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gtrecagts.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gaofsvpua.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/grmbhjltt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/galqyjfsa.sHtML


<!-- 参考信息 -->