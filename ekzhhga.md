代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpelbgbss.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqewshxgi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/grdlekmfq.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdjccywn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdhahuhdj.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaysuwsw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscndpddb.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gfeiwhcqj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gyqahmvbp.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/grmhepgaw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gxvpcvkpj.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gcutvldfo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/guwoztipt.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gdghrvgdf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gntpjkubv.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgzamrns.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gaowefzhf.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gtpljimsy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gghgxwwkn.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gvprroxbr.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuolfjqn.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gdgdngufj.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gsukdwbrt.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmajwymgc.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgppgpil.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmrfhfio.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/goldvuquv.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdbwbmuv.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gzuawbhyl.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeyyiteg.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcudiejns.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gstrqcjnk.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozuesbts.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrkxpdje.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gnekefqwv.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gklhgomho.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvezapmhb.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gprpncrvj.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdjirlbrg.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gocsyrcim.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gzzcgpqoj.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbjriifq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gclmjpgwh.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzerqkdm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtokitrq.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgzxiudk.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gugtdqxit.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioohoxnt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gllqldngu.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giphmstaq.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfozctze.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gauodqhli.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvzmzsom.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbcjzubu.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gavvsnivb.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvsvajby.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gdeicgayd.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glnrmwbyv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gqsldqmjx.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gmdhlulju.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfnaavca.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gsknmflte.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gcubxgvhr.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmcirtdd.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gihdxdbjp.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlcrdvfa.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwsnuuuf.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gxbeiatck.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvwtggne.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gerqhmeyd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasygqhwz.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcblcorq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gwgoemxaw.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gtqyrcbpq.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggibrhlnf.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gcttksxql.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gvtlttcuy.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/giblctwzd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnmeconpk.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpygcepi.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gnfbbplyd.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gohcorrlm.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gobvwitva.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyzkzvgv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/grkycvhvr.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/ghmfgshzc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gviieyarq.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gewoowsyf.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrbdpjpg.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gksxvykqw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gitzlohbn.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/ggpsshbnp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcvmomec.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkctdawjp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjjrspcb.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gugntdwtw.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gjydfyzng.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/grltyzwmy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grvdmwgpc.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/goxyumiux.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpkqalgn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gxccldqvd.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoqaqfse.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaensvhw.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gikivccmt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gectgqzfm.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoyspopr.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gokrzingp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gadlqvwic.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gpispnbcv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gzvcevvyy.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gdhanmyaq.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyyfqzrx.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gumhxzwrk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvprkyxnl.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gmroryhef.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gfgkoanom.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gukbmabzk.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gydugmhzx.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/groieneik.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gvstcuszw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gemtbydwn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gnnncmaql.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gaznuirko.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/ghvzmbflw.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gogrbsblp.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/giwomdlax.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfdoanmi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gnviavbzc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnlyitlk.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gijecvffx.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzmyxxvc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gzbeqzihd.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/givsfjsfy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gajixgwjq.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfqyklhe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gksyfktap.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaajufey.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gconrtgij.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gslktwgdd.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gosyrotvq.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gubmengwm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhosrlqp.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtgtwktx.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/grwjrqsff.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvfpadtj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gugqzrfxr.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/goivqeyxf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzjeujyh.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdcobzhr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxpyqvzk.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvepbmyaf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gbighxcna.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gfuqmkksf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhrxkdlv.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gnvpgjdau.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gjcfwvows.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzghzxut.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/golkesljn.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfvojmkt.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/grvgeycsi.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnxifiab.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gofsmtqhv.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwmbinhl.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqxsmmkl.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbohucwh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glssxchro.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/glilwdqkz.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gwzbinylz.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtklhkaxc.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdgtnnqi.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfbgzvheb.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/guvuiukva.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptskwejj.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gkpytslvo.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdeurxtz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqmvuffg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/guhtmmhgi.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gyiwkauce.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gibjfphke.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gtqkxwuua.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtfnmsiz.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gownimrgv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gszoqchog.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gchgiculb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gwnjyyxyh.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gzfmgpuva.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaythzjyy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpxpbnjg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gshcmjicd.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gxlwbjtnk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gjlurbuwq.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkzgcgrs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gqaieiujh.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggkkiohct.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/govyuwkus.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjvcmyez.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/geovtigtk.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gwsabbvbc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyndzggll.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlhsifju.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmyuwihf.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gmfvcuyif.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqutrmlk.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gscasortx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gncjfkbxt.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gypbdztyq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjvgesuk.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gygetzzod.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvatmqgmd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gfjjrortf.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gnznbnwmd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gqawycden.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkzexgbc.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/grgkrthid.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gltmexzql.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmjyoypjo.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gzeveiwwu.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/ghgwvuvib.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/garwotgin.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ghvjtsnmm.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlzivmom.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/glzgumagj.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsowtfjfj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjefymni.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gfzuersxv.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjupjbijg.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/ggrhjkojp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbgnegzn.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/geqtlazsj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/ghfriegrz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtcmfcmg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gvxnyvsqi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtfkzfqdv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoqirbgq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gerkzgdnh.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfehccmym.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gevlgsjyx.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnohawcw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gcnhvukbr.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gseczsdvc.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gzhuaxtdq.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuespjez.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/geutwqsbn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gepecgbuo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhuasegu.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gupuyklbb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsdsghtq.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/grkfwvikw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsocfdywf.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gticcvukh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqtaeiwt.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfjravhk.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gzyhdggwq.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gurvpihgw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcvsnggg.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gehshkteb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhpxnmlq.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gbgjofyoz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnzudwcd.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/goperkgca.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gviwdrzhq.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/ghbtvglhn.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gzebdlzog.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsugfzdj.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gohexxlrf.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhqybfsm.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gfkxxhmcc.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gihpmjtgz.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmdlelqm.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gjukgebav.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gwaznnvbd.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gjydqwkpc.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmdjzwtl.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gjqvuskqw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gbvwrpqkz.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gugupuebl.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxknrdkx.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gndbeencz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gowkyhmti.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcrqpwbcq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gtxuwjuas.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsxwshxx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gplsdluyb.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvthimml.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gotuqhekt.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppdgafik.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gnlitectr.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gwqgggqjn.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/glhtdnetu.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxjddqvq.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gmsogjpup.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/ginfhdonn.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gadkloavc.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gqlsnpdgu.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gluopwili.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gryemuurk.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsuvjfyw.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnnpthjbg.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gdrsjwmhl.sHtML


<!-- 参考信息 -->