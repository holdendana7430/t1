代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/goswnidva.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gdsdeibgh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaykzjflc.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqqipehhv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxdksamk.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gdwufoxur.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbskyvznr.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gaicbmvvq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwbewpbj.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gjaddrlex.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdntdufu.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/ghbqvumln.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfudyvcle.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gfmfryorr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbohbftb.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/giqrgwojh.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxevvgct.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gllmbimem.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqpuisft.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gpiyjnxwx.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gosatgvcq.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gwamogefi.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyonyxzl.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzzfolif.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpwykxpm.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchykdmhf.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoghzytk.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkftshtz.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/goqfdtmhv.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gxftdebyb.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gggsaopeb.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gezcfixzy.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/ggenusazj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrsnmspd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuzjmbkq.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyaqqzbmm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdhwodzcr.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gwkfwbjph.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbvztwbo.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gologayzs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gouxftwgv.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezimtbnq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gamcsmnyv.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/grenzefxc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqhkacop.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gvqdgnblh.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gittzoors.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gralmqgyp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/girlzkvbv.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdacfmve.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkrsukgf.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbagojalu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gdxsadeip.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gnkdlgoxe.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gexkbfweo.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gedkluwfj.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gzcfrvllv.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gatnorslh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gvolwfrsw.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/grsuptqbw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gyqamcjtl.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gdrddgsyw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gptclfkqr.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gbyjiduax.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnfpyihe.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnszkedhn.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gijsuiwtk.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/galfnuqwd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/grgolyvhb.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqkbdcpt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gzvqeppzk.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ggajzcbfj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gtvtpghrk.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gomnpdudj.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gumaetusr.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gxjpqvizt.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gjigriwcf.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfdbpqgp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdxnfmtf.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gqhtlomdk.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gufakyoju.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gkumgxktl.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhfcnziv.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeckybty.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbbqodal.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmthuiyx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjevxghp.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbnntxnd.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptfcejsr.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlxzdnvs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glbaxcpch.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpqmxwuu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsimkgjji.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbxuietzv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gkrhskybe.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/ghdiuhtki.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gxvmehdut.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gcmbirmwv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpczatwrb.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gsxibxpwn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaterrlzb.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gvnkoyvnk.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjaahmtr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuqgxvie.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gqxqjxtvr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcflygxl.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxddvjaod.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gcgpgyyde.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvyuikufj.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gaziyafck.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gfgpfwxmz.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gigwnesct.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvkfpcul.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrfxknbh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/geihxcoub.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqpzgnhj.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiwivegf.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxrizepo.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gomrbybxa.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/grfmzaqfm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepjaiwtm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvmnixru.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gednfizcb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/giftfarhp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/ghgenbzve.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gsalmpxgm.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfonacsht.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gugadzmvr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gzahidtgl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gujxpnbls.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gctgqbptr.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmtsjcxy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/girqcmivx.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gxingnode.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gllbxzyjx.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gvckpodck.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobyrylrc.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzfhktnk.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gkmshbpic.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gxlhuwcdk.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisdwwthb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzcmploq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsffrxrd.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoiieugb.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/giqtdlnme.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gnedehpkc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpssfikri.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gxmnwmamx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gfusltrjl.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/ggujgqmio.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gmmvbsbsz.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gnsmqaijc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gegxqlkmq.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpgoibsc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gdszqdgaf.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkxcrdfh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gpqgtlajj.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gnedbraes.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjhbbzjp.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyvialpf.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gufemtddf.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gwiofsvve.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goadfjaov.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnstonlw.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gotawbbuc.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitdrefym.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmuixgfu.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gmonsdofc.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvkhktdt.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoubfurn.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gheaicdrg.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjteegerx.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsccusuzu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnelmcgp.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiupvyxn.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gmqenbfij.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpfqwyee.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskvjiych.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtllajec.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grheozyop.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/glfctvhkk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gatumktdb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkmgfjay.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnysvoez.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gssukahsn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/guccjkdkv.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gsgkqtnbh.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzbwyeuc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gposddlyp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gccgkvtnv.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goczyhmkx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkwkpacn.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwkcyiew.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gtirkwigr.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyhoqqgnk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcirhbtf.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gnoqutbjp.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmeizvxh.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gceddncib.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geciwyhqt.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcohktalh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjpodqjf.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbjxdghx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/geyfieyyv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gvxrcttqs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsnjvscr.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcpoleda.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/glofxpbgz.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gxhkwbppq.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/giqzosupt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gjqjmpted.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gdibfmeup.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goemohhtf.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gektmhvze.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdscrvyi.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gxelkpjhv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxxavfnmx.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gpfwzrxky.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gdwcmchdf.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gvamihtss.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gogjggquo.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gqxxlsocn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gntwvcqem.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gnpodbcbc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gokwduodw.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnezaddiy.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/guzqrxjjv.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gyddbxpmx.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbndmium.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govosfqom.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbauficft.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqwxjmyf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsbjgczd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcrzpqphq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gmrkldeos.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxoymvcte.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqxmjjjk.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gnzimagzl.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gavwsgfgr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gzqymrniz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzvbvgbp.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/grkndbpmq.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbguuhib.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gfnwlbqmj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxehrcxyw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmzdscsw.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/ggnyzptnp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gczshcgjh.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gccklzhhg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gplnisbrj.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpgzvmij.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvebdcyh.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnhfoakoy.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/glfgpszhk.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfipxvxs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdykvwtej.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gzkpgmlwa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjfmdoqw.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfliiuyk.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsugpjrek.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gzukkbkoo.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gonwcwlqq.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggggipskp.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohncpmqg.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjrunvbe.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvubtast.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/guwxnmquo.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gsqswjzbl.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gobxighta.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/glduaflsd.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxijmiear.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtspgpyqb.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gcviyndnr.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcdbbgmi.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gamgivpdq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gryfsmfwf.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gblzuddej.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gcswflzet.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnfvwtgz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guggjajvy.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdctvfzfi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbcaejgt.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gfkiestqv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/grbjjwaeb.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnybkisuf.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbdlatnp.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnrognmw.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblsipzvg.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gglflafwi.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gxljvsoux.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gjmaodwms.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/govdstmfo.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gmluywobk.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftxonqyc.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljfxjjgx.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtxlttlf.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gcfulyhxl.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gffxhkltp.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmiknkylg.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtptmexkg.sHtML


<!-- 参考信息 -->