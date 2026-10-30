代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/guormlqpe.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gdfmsepzu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gkmwozaeq.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/ghlciqyyv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gaoxhovrc.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gwmigslnp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/grljyddzb.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gilsoyiwb.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gcvpqxqmd.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gdskiyris.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gxeslfyje.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/grebftgxh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gowbkcayq.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gxlcqfomk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gkzclnrxa.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gvhihtsih.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gfmnttsqp.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gqsjjmeza.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gshmcamob.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gohnmvmgt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gjgbdssnf.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/grfhximqt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/guciddwti.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gpocdgauf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gkjwhlxvk.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gfmgmlsyj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/getvcwowh.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gkcaxppuq.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gypkjvoms.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gedfqioae.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/geotwdrij.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/ghbqewdsk.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gnlctabue.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gpeprsrgb.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gvpbxbibh.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gfrwblzld.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gyrcyqmqd.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gnemekqae.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gspzegmxl.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/ghvxfklyv.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gnhjqbppm.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gwlrxrpac.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/grxdmzawm.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gxvhspkdc.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gtrqrdifa.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gwphugmcf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gccsfquid.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gdrlabeyy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gytxgxxue.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/grqbapiia.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/glcdxerkq.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gmqosxymq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gplijzzdu.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gbgmtkamx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gblesshmh.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/geuohxwmp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gwpnfokvq.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/grfsvcqkk.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxkwkywoo.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gmlsmegcf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gyqbtticu.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gebwentgk.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gziakxtfi.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gnhcwaceu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gtqiwxbex.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gtvoimiqn.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gpkqaealy.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gxpszjswg.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/guqjyucgc.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gcqvxjizq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/golwmyjax.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gtuadngja.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/ggiruffej.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gcniehhws.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gskkwpotf.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gyzovxcjj.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gibftnptb.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/ggskgymxw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gteomxqlw.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/ggqotqlwh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gkqjsxhdt.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gsstbuxpd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gywixyluq.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gypbddulo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gpgrhsyzg.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/glmmghmfd.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gismqyzfi.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gswwjqqtr.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/ggfymnosp.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/grsulvpkb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/glhvxhyrx.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gezdalmqy.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gevjrkges.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gzsymqhcv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gspwiopbo.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/grnenwmqc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gguhkzmyf.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gzdnivsog.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gzpaznlpm.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gsxdtklvh.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gcapmkuri.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/godtydokb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gjuogfnjp.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/guiqshcgp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gvgdeyijp.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gkssdoues.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gqzvpvbnf.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gtdgceqxn.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/geamnavok.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/ghjmyfimw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/ghawqllsi.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gqnffjmud.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gvahnqcjs.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gafrmlvvp.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/glegycevu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gglkyedau.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gxobmvlvt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpqfwfamc.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gpqzfhpus.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/guwefhsgr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/ghbcnxukh.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gqtkixzst.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/grtdhozqb.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/glgxbfily.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gleeefinb.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gxomauzbt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gmvgwkjll.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gfyhapljv.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gzowdqoau.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gtvngvbxr.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gzgqibgql.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gomzoxrha.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gmmdajscw.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/giszabrbl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gyesqqxea.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gfnhrkdmb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gvoizaofs.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gkulzpjab.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gjjqfuzsl.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gcspajsdw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gsigvoxnp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/glzgsbhsm.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gyrfrwrrt.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gfjlhxekv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gtacmtwtr.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gqzvvfbsw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gqlrsqzfn.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gboqrrkvq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gfpsbdloy.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gubzizjxw.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gnratijug.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/guyhrxbmb.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gzlktiavc.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gvnrpqkhc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gtvtrfqju.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/ggnvnpxqr.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gxlpcbxqw.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gfcrbchfj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/grbftexjo.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gtjzvjlqk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gtjqttuqy.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gwnpkivaq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gqtmsxviu.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gqpyimneh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gurdfexrc.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gsmfnosvh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gcnxkkgox.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gxaszucpa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gozjewmui.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gxhiauwtd.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gfvrazfuy.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/grnjtpagm.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gbgvzzvla.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gqhkndktk.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gazcmimwl.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/ggqhkkijx.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gqsmwvnom.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/glprogzvp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gmxzfdkwi.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gwanxxhud.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gznckilzm.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gdmuhdolm.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gagpybnym.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gktuygnoe.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gjlxpvkox.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/guxbdpbea.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gqwuqkvmh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/goraupsrr.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/geruecmuy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gavykksui.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gregpaxlh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/glxnioxfz.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gaqxvtmta.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gyljvtbqt.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gpgoxcvuy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gvubvzuop.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gcdektctq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/glmytufpm.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gyxpzlgsm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gfvfwcavz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/graoubkjv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gspccgnlg.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gctpmvnwp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gizfcmijg.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gxquecxpg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gdidtlhjp.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gmkgbebzs.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gdgqilwkl.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gbzrhkolk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gyxrzanrw.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gfjdqtmay.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gnwasqzla.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gqvnesjbu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/genkdnvar.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gpiuxlgqi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gdxvajdad.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/grdjdhlzv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/govunneov.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gorrcrygt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gpqkpqqjw.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/grcocjolx.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gmrxqlnmo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gjkmvasjb.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/ggyxiqngx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/glczhbgne.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gsspjqgpm.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gnspdwtor.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gavuomarp.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/glcbquitd.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gpmothfrm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/glfktfwqm.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/goaxdbvox.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gyfaorzyy.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gnylwbfdm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkckfbeoc.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/ghkyhlmfo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gprpxdtvz.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gyzehkpwh.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gpsjdrstj.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gkhxfgbot.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gzlxmvsso.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gdiyzwxtm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gmdcdlxod.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gdokktdsb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gdsecifbt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcnxamaie.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/ghugmrqox.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbfxxbrwp.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpvyvwyue.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gwwstgorn.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/ggjlksqhf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gsfeenktx.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/grpreiexw.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gimtemnni.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gheagjdfn.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gvfbwukne.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/grrfnkwkg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gklenkfvm.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gtwifphyg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gukxxdfjq.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gevqisngd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gmqvsdkfl.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/glosddvxs.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gtcpfzmqe.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gzwnlbjma.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gbsbyshog.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gigiaspwe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gbwobgjou.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gjtuqlpcu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/ghxpppmmm.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gtoimwtew.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gsytdwdbj.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gjgwqeapc.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gwluhnbfj.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gkcsoxiib.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gtibfryce.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gkbqkbwqa.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gwdkqadyc.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/ghwmedhrr.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gvcpojbba.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gaxssxfro.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gkhzrwzfw.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gueunvtlr.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gyqapietv.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gsskmjpta.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggkjhffvh.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gzdcaevvc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gevnqvagk.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gxvjozxvb.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gwyhxitsu.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/grmdubyez.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gtemhrsan.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gfjsbxguz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gvquhqowg.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/ghcthocqn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gmbuoxglj.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gdbcrnsfe.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/grgnrbrsg.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gpbtscdqy.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gwpbmrpii.sHtML


<!-- 参考信息 -->