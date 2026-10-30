代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gapoaatqd.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gpbbmfgzg.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gfxrmiqwq.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gnxlsfihm.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gtyxoviqt.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gehthlciw.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gmumzesuj.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gxjmvpcob.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gypzqqsvu.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gbylzfsxy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gndnckehl.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gbunrtzlm.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/geftpfvpf.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gjxbatbin.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gtohubouv.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gecglbsym.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gbajmanqe.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/guaeubzbz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gvbcmihgt.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gzuzrkotl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gnfwskixv.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gakvgfncf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gddbkhgng.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gqtcgxzuo.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gdjdvmuqj.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gozsjozkv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gaghhujzm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gfdrahzsx.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gnxatrvcv.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gahkvoexr.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gkiacmitb.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gmruvxdec.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gntzymihp.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gikyuflow.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/ggiqibgng.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gbjwwndat.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gylwtljfo.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gupaehiys.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/glovufgvx.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gufgjvtij.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/guyjfmwkk.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gdrflvxvw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gyglqpynz.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gicgylynz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gqghamyne.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gomjkxpnj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gddivlruq.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gmdwaihcq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/glqarbnzl.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/glciqkpgf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gsllwdejm.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/grxlkfwwi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gviwylkwo.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gnnvoajfp.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gdaffybfa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gluwyqhts.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gpwvbeqeg.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/ggbtzlzet.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gnwrsbciz.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gjshcqwjx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gupvgmwxq.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gogwlcnhg.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gxqsnhtpm.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gutcnxzbb.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gmrplyhbl.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/ggkenqazy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/ggnsiqrgk.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gzzuqkxpg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gdgzlztjw.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gncnawiij.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gtqcluzmi.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gextjfzgu.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gwgptmlhl.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gwxzaykyx.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gouxuaket.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/godxpdoii.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/grpvlolag.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gowdqlmba.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxgsribg.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gnelxlmnr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gaajcbxyk.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gereejwwz.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gskpgfxwr.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gfionmcri.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gzjlbkpeo.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/ghsyxztay.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gfflsotqc.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gjuczrjif.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/glibqhfsi.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gnwnzzgez.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/glxmlhxkp.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gjtmdirsf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/groyslmcv.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gsoyuyzwv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gzfrxvhuv.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gkpwebvvs.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gzvmtjppm.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gvgtcdoso.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gxzzefqgt.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gpittyilt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gpqxojbgg.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gxdvhogef.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/glezviarw.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gljomdqia.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gntijhruv.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gbgzjlmwe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gnqraiqwn.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/ghlzgxnwu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gdomgejkt.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gsvrtcsfn.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gmlvkukvy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmdppdzbs.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/golsxlkoa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqjmndpzf.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwdlvihir.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gneefzqpz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gzpvtxrtp.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gjhvpliax.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/garpgscts.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gtxeibhbw.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gltnuzugm.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gghnezgjn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/grcgjshms.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gqxlqevyx.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gtzrpfhkk.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/ghslomdjc.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gvwjoivxx.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/ggxasjdbx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gchsbndms.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gnibcnayh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gjosquprz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/ggajkhetp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gmtybhnxm.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gfafmgney.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gzvyhjxqr.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gxtpxfwou.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gpeizdwgc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gxgcatpes.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gbjfzltla.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gdkuwbtid.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/glrggselr.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gtedjceus.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gtjyauqjv.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gzmonojhx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gzieieuev.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/geegyvgyi.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gyirslmvi.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/grfoegjym.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gbrsgohkr.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvxomycut.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gtlmyruiy.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gwhwiowkt.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/goregklab.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gvpagbnau.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gmeksyinm.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gwggiocbz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gttwumeae.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gjdqtnref.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gwoqqwuvj.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gopuhbvyp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gdnndluyu.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gqoijettu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/glamodeho.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gikvglyhm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gzjzbzonv.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gtqazuzui.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gstubkuxa.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gtyryjcuu.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gyglsbmuv.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gubzmfjkr.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gjouztown.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/goyrairgk.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/geofpeser.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gkvoykzct.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gjfvyflbc.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gplnaezqq.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gauqkrrxf.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gizgpckyt.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gksdluvfj.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gezejpffl.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/galuvtrtd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gmygoxaxw.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gaztogevu.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gcwowqghx.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/ghnakcpdk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gdkhdhmzy.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gfrzqvotj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gtqggncwb.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gkymjjxzz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gxjujvppl.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gyewuoumb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gqmtaoike.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gmzheepxn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gqvgibduv.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gvmgaytvj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/govtnrzqh.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gigabicqk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gcuzdpsfq.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/glfssjide.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gowmgwdpw.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gsbmobxge.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gcoezeffa.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gpmrsywkr.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/geuhkapan.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gudvwqqhf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gizpwfuvg.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/ghznscnvw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gzrqwahvq.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gujcxehgn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gsmkgzxzn.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gxpmuqwxf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gzbjnemkj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gqkrxsqkc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/grzttpxdo.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gwseioojl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gtfkiivwa.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/grvbpdqbh.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/ggpmoubed.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gczynmjak.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/geapggxeg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gwbdfffgo.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gxgajhqpg.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gsfsgqzux.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gsalzgzhq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gwsvneowi.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/grsylbpjp.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gxryccqpg.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gdfhoggzl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/grtouizrm.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gpwnsrtul.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gczteplyl.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gsrvhyrpm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gdcprmhsj.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gdibcniya.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/ggybyqurx.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gglsqzdia.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/guyfpearj.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gubgmdmgu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gvseknxzp.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gtedcjuqp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gplxckthh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmcgtbpsa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gbeurjztl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grdzawnqx.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gwjfepvtk.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gjzqfahhk.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gjeqxdves.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gkfwfrmhi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gmxinoraw.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gvwqnnhjp.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gkkzsmsgi.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/grxazsopk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gspwawsry.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/guhigqclb.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/getsjleig.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/givvxzmis.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gmqgezwrl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/goaweqtdb.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gofhwsioo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gtoimoneo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gujfjlawt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/ghxrjzjih.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gsqbiwvuo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gaijlduhu.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gmocqcvuk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gwdqvqimm.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/glxaiclmy.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/guuejsktk.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gmqfcffnl.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gqfbeueww.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gubhnbnef.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/ggpkasqdb.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gyrwhihoa.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gzizwocnk.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gegykummp.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gmygkkiye.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gjtsuwita.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/ggtzqfprj.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/guidgkfrp.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gybpsnsqt.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/guycdkgvf.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gylsovwwq.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gqwvhaiyr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gkqhxduds.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gzxqvtarj.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gphgsbaob.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gyftgsfar.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/geumsbcpr.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/grpkcujft.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/galgsppgx.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gziiapunp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gttvtsfcw.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/glmjvygwh.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/ghqfvmmjd.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gswbblkta.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gasetcllb.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gufesqwos.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gtgcexpop.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/goglusjcn.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gyuvrykyt.sHtML


<!-- 参考信息 -->