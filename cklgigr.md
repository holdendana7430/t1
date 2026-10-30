代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gajcyzwpd.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoiwnqnk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxejcmwhe.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gxomdiezs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaqpnvmg.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuxgkoqh.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmdojska.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaitasjp.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/glgnpotjd.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxhofjxm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyumbdtg.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gswvbdxsu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrwdxhms.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gunxuundk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/giydwoxij.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvtibpzvc.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guwtqntdd.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gffdtipib.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkzduquyw.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gvywflnex.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gnilfuljn.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gmujvttpv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/googgfmhh.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekzyczfr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gutqhfynr.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gbyzulrbe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsppqysep.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcslfilbw.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrmgpupa.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gxoygysxc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyyxnpbt.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/grparcycy.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gpitjurkp.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqrptrae.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjqlpepw.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmflzcah.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaezrexp.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/genbatnwy.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpdlvzxmy.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gndfwfpfg.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfuebzjx.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfzfjsoo.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnqqntnf.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdfbsose.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gttmednks.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gnfklnvnh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gyfwsddkb.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxgmptqr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbclrmllm.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfeepdwy.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grijqgpok.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gahteeiim.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gyypgflev.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gxgfzwixj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gulnpabxh.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gqdcpaqen.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkmcicbe.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gngpkbqip.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/geenzjpzb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwctdwwqj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gyurwimwn.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwiyjpzb.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/goliiaupj.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/grjcbslch.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsnicmao.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gdzvhrwhx.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gdstfxkkj.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gfqlxwulq.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gqnsqpnya.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbmcsqxtr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gjinqdgne.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaomstst.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzqajsvq.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfisaexmx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/grsngenek.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gkijqlxpr.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpytjrkl.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqmzoekmr.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gllrpjcwo.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gifkdowzk.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/ghdoignfa.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gesuupvwc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gktuceggn.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/geyisvihc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkppqyoc.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvftskmlo.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvmgezeo.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxzvovit.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gltlpcdcu.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gycekofgd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gluhsyaef.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gkovcibvc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/glrqrrcyi.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmckctzf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvtkiflo.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtoebznr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godmfuife.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaksbqfo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqtjmmyg.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwsigvvrw.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/grvybtjoj.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/googycilw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhyapmoy.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjwlftztd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxeldagn.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnukcgzzd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gwmwnjlia.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdrnybws.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgqdqrir.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gqatwkohw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkozfzvv.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gowhppmzt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoydbevr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgoctiar.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppmemhjl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glhpmwvfy.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhweapqr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gghwazecu.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gtbnwewcb.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gsjtfokow.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcgnnyog.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gjrrwjetx.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhguosdm.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gkgrdzanr.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjgdledw.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gldkxhtfn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gbrnhvskj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnmlfdwx.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwyfgqaq.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcfxsved.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/grespluew.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gcqfmaeju.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxnktmot.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzwjpkqx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtsirgmn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwmzokox.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gogzlpcux.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcqakxuu.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gfjpiuvqr.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/glawusicp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gfsvupmex.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/goxovjmpe.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgguuicv.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkqsmive.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaavakfyj.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcsbcfdg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtgzitwi.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjhpvsub.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaurrnzi.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gejhnrtdb.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpamrdqvx.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gpnjolwrh.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyrhntse.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkvmdlow.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gxmgttwto.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkusvmzt.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwycplgc.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/guukizgtx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjriryboq.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gntjhcdou.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzauhksx.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqkwocvn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gbpaoveqc.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/givhnkylp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvamwsam.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gjyslzdzn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsqtjztt.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmfwsgrw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gtozsttfh.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gtzbfwnin.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggixqnvbv.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbluswhx.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gtuamkdvf.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsfiqwnc.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gmzvfsmcp.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdulsvkvx.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gcoxfyxyw.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggzipwesi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgmcewyb.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gxozqcbim.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/goahestka.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ggghzmmaf.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gydrurowx.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/geclxacpa.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaceescc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzssyywc.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvitkklft.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjvlkhsi.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gxowbkgpj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzhoawat.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gekvksych.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmczrnzs.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoekmlka.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gqpyzhctl.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymebgxcx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/girkkbepf.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhtkviaa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gqcohlode.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gwkqobymb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gfomqktmv.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/girboepjc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gmzvtrhtw.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gdabolael.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/guomeisdf.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnobhjolb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljjqoxgm.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gagcaxnig.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpxzgnxp.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gojhdknxq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzescthe.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcflighui.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxpzwkyz.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/geyukhamc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gsdgfbgdj.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnseftmf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlxozakp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopwyvjzy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glixehige.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gghgmryry.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtptrpir.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsinffphx.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gywcodvny.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/glgjacwtc.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggavafjiq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gnytlmtnx.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gatuukiup.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gfhttgeaf.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gxcxfjacg.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giqzjeivl.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gvqlvwizb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxjysqiv.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gmisboyym.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gsdycqfay.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gsidwnrvh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbichwmzr.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/ggtyfverk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/glglhxcum.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gueromyxg.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gykeafgky.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyqhpcza.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/grzwefxyg.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdzlcorl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/glzbhrift.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvvyhzjc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gseprbbvn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggcfpmdcl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/glrxpktnf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gidnbqjvz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grmcicigt.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzifebwqx.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmtsrhdfu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gcfsaalpd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyxckbtn.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdthbpsc.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gaeosnizs.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gogzynnpd.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/glivmlhiy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpikaaoh.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvrurbll.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazulvfvi.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gfkzngnkl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/grlinkbpa.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/ghucrwcks.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gsoadhwnm.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzfgcbye.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrvazdrv.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrsojjdc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gyhxgwmap.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyojdzxif.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/glkegvzco.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gxchixoiw.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/ghcmfudsz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gebrastnk.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ganrznsmr.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/ggdpqstwy.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/glgaeinag.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbvzjkau.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gojhignzp.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grwcyiuum.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiyncmup.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/glduaafzz.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gueaaamof.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdesrdkzg.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgonxwfa.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkudogtd.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/grbmpozur.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gnotuenno.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/glpmheofr.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gcgojvkta.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gtljfcsjp.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gszlfdlth.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyqmicpi.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/grhjnxyim.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gwremyjpg.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gehiwvhup.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gseydwjsl.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceqaxyox.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gowvrqped.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyqvlosn.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtautjwf.sHtML


<!-- 参考信息 -->