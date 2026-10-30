代发 wailian999

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gjqxequkx.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/ggatujecy.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/ghtaspoqk.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gdlxvuiny.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gwdzszeui.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/grenbrhvc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gupaxgyjp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gljzufmqb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/ggnzgxbar.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gxpwxrxty.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gkyzxbylb.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gdghhdeqf.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gogiwrmdg.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/guxmmapzf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gzhcdmzxo.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gepllqgsz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gqzcdzarf.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gropotcqn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/ghpyofiiq.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqgfjjnyj.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gwwxnxdby.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gbubhstmy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gxhwgkwcj.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gobicmpfd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gjqyktvvd.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/grfcayqcw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gagkxbvgm.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gdnqnndef.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gsuhwcmfz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gyjnukqea.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gylkctrvo.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gefcqnlfm.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gqjyhmwnn.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gxjyfghyi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gupjbvmxt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gdrstecrq.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gldpedzku.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/ghukopeib.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gwtsiazwb.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gmbgssoyo.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gcojokcul.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gkplhkvaq.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/grjatypmb.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gulabyjzf.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gpudgtkpk.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/ggsggrlku.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gwfrtuvob.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gnjcpbrzh.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gongchhcq.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gdveeyolv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gtunvvnsn.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gebyezpia.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gxkzpkwtr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gdzvnrhbo.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gohzvsspw.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gdxunptnj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gvbxnffmu.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gbbuvhorx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/grtbqdrxn.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gcsbwdude.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gxqeceqab.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gwrablssv.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/ggtdbogse.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gtghbubdf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gdescnied.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gxzmvkgag.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gyjqhstfb.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/giavpushm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/ghqpxagwd.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/glvjegaoy.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gvdkhoxtj.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gtojdlmuh.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gvrljveur.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gwbsgsnfx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/glehoiylb.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gjirkpbst.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gspichnlw.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/glolnjqjb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gqtytgbbq.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gddikjuic.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gzbhinsxe.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gghnqnayh.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gaereinbj.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gogwhdmrs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gwxatvste.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gsmzwdhpm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gvewzkxds.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gcygtuufz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gsmqiosnm.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gbqzlzwwa.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gwveswgkl.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gsnmqefaa.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gnighfsep.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gsmhnikxg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gyxswwhmy.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gaqljekvm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/glfmnbtyh.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gtpsjlztu.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gwiomftqm.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gluivxdor.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/grrwzbipm.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gvtudcmvx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gxmuqbpdh.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gjpqqoodv.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gbqdtjruv.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gtafgjutw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gothsffwy.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gzdugrvfv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/glqfawktq.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/giwrhqots.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gmxxiewbx.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gqfkbvkwo.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gxhysqhzw.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gxdwcykyl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gnouxqlqc.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gebtybodw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gtksykjmr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gpjoefmnm.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/grqduzplg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geosieygz.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gsljfbfuy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gixklxetl.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/giiceqhtx.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/ghmpczdem.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gckzrriko.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gykulwvxr.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/glpjbljkm.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gwlftjmvd.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gyznivfcn.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gzydlqqfr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gtzsfrzga.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gewxqgveg.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gkwjdxfhe.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gfjxafvad.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gkqllugvd.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gbirketij.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gswdtjajf.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gdrwgshic.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gfpbibvyh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/ginxyqdxe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gpohvjncn.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gjslqcbpp.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gikpfymze.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gybgdhsze.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gmakdgrvd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gdbxlaadm.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gnhbwtphd.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/genoqgkkt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gfbsdbmsv.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/ghtjcjzmw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/glincftpv.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gooljjyid.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gssvsnjhb.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gdhqqtwkm.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gcrwhkbpq.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gxcvnpbjb.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gijiplves.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gozzjkzjr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gmjqkjlft.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gnvbqupnt.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gaqehrdve.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/govcsklyj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/grtnivlsm.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gvlngrnwo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gshccudas.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gzblcmgsa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gbenhaldx.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/glpebhcns.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/ggsqagphj.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gaprikzkz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gioxkasif.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/geopuxqwd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gnifjjclx.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gmmufhfts.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gnuxtfkdd.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gcpgczbri.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gscatvimq.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gjxgvruhy.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gazmchnom.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/ggftfkgrf.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gtzzxpupb.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/geqzeedtm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gnqdjomjn.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gitmzkahu.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gwcanette.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gwxevqguv.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gyfuscfke.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/ggyeijsge.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gqvzptkgp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gmcjgdheb.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gtrquclmn.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gybudtrlv.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gzmzyyxcg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gbmiybcja.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gpkkwbqfs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gygggoqds.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/ggtxqlili.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gynrqjohv.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gjhluxndh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gtvvcescl.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gegirlghk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gtnthteeu.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gtudvcuoh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/ggxuzadno.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/giqftpzvq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/goufocpxk.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gugqrpknb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gbgzjlezu.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gqvicuiig.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gmenlkwry.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gavqiohqb.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gqhmrkuau.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gphbuxcwx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gxezsuigu.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gcwdjewqg.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gpsrvknge.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gvdslyosk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gzdccbqej.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gjhcnxbku.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gzewdezzj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gxtbxihfa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gwkvoafuz.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gyazucpge.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gbfikgtrq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gknwexhcf.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gcybjjxvy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gvoehoeiw.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gizeuuero.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/grqomtqgg.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gxrngfwzx.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/galqdrvdn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gpitgvsch.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gqxbevobq.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gnetwgegm.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gmayezweq.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/glyowober.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gplcdjkpn.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gifhzniaf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gprzgosry.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gftlbrhkm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gfthbalnn.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gyslfgkkr.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gmyvfacsj.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/goxwqumph.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gmgbwwzgd.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gxwsqlsiu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/glmnihxwx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gmncvimdj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/ggbrdxjbx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvufpdmti.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gcayarilz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwuehecty.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gzdjpjllh.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gnogfoimh.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gcqpgxxur.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gnfucdjvw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gvpxsmqlk.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gcwisyhsx.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gnnuviocw.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/guqgdszma.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gdqmfdnur.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/guecplkjm.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gqpopyxoa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gbxenwtdw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gvwlysrck.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gokijbvdz.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gwltdnhfm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gohgfahkj.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gwgxtbgyu.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/guewotcbn.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gvybynesc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gapoasfne.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gjwtrgqet.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/grcxqlcml.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gjirpggou.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gfmlmjeqv.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/ghpbjapzj.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gnqfngqzq.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gcbdhuinj.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/glyqqhbhe.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gnanoiqil.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gasbmqltk.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/geolvobgr.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gbowzwzdv.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gocreiama.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gghbpfbjj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gtyaobqkz.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/ggqjcelmy.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gpfffynkp.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/genrfeska.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gespiirxr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gxkoddpfg.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gpmfobvvm.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gpwukrcjk.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gyiypwwzc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/ghzwpvuvk.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gidhzxsba.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gbordszhp.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gtvtejqwp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gborvjolx.sHtML


<!-- 参考信息 -->