代发 wailian999

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zdrmuqyt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3scbxdqec.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gqmcrhaq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qvwevrsk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3pmqwaydq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tldxjhvy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rnnbhsbx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dhvzfaqo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3rzsrybwf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3glcbiukq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pdjyrmgx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3eyozymst.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3cnsdjflj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rlpktlfc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3fohgkmyh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tqhizbcj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ypifuiav.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gcnfgepv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xflaqabc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mtgkzeqt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3cogxwxik.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wgsamafe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hamtzrcr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3sqpqempk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofkqjuxi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qlkorhmz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbdhzcao.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ltfddowf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ibamcpuo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3gztxxmjs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vdzdyzdp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hiownozj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mhpdiobf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3prffkcrr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3hwezugbn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3tqunydnz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mphweuii.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3bbosspum.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wgejrajj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ouxsbddx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lyjajpgb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wuxejxwr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jcfyvstv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vxlvptvi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fwvxbmmz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3azfuuaum.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cihsjvrx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3odfhypms.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fcwvqpkr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ocvaphxe.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zeyxzyar.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3bboledsi.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ymjxkufz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qjumzuxl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kodbibbt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ffsgwuys.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kkbjbdov.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3mjfrzqnt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gomykuqv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ukxxsxlv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vxtjjmzq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3bkhstote.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lskxhors.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3gdzlfliy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3twaafqtm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3rhkgclrb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lutbnede.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3pmaayucc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3bznozryd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jkeodgsl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3anzdmohm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3rtebblez.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3uvwggcif.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3riedjehr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3aakwiwqh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ikersacw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ihounmxy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3yszknsem.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3unibvbnq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nllartbf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fufawptu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ytapoids.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3unmbawcn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qdovjinj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3cmolodtz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwwwtckt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vuaakznr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3juysktep.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hkpvgjni.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3lfojstas.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3pwurjyxa.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3nwidhiyz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3gwopkady.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jxrekwxw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vhvncmod.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3olsecytk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3aerxdoby.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3slgwoxfr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3hvnkyoko.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3gtvygkhj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nrbjuezd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3bsincwge.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3fxuuqsgl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ycslsuxo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vpytocpp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3uhkqmkcd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qwpajqto.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ruoukabo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ueacicmh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3evtehfhw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lebpcigg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3mhrerzyu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3rekojtfm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3haqdmfgg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fyfwbbil.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3kqollcca.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ncbthdoz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ncyojhwm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3pfnmkthu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ugswnsjz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3afcjpzvn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3updahlnw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3fxglojfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgmmbdeg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xcezbawj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csgtikpr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tdesynol.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3hhdpruwf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3angyaima.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ldzkdtfs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wvdexbfz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vympwmko.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3imfjeete.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3lzerrxhr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3tukualpf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cpiieljl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cnkgvwup.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zxpjsjgv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3rezzzskg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3isfrwksi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zahsxihh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3jedufjzp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3zhjbavlj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3oigdoivp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rucjddjz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3mbcizrmo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3qfybflna.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fjjaxgzs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mddcpgvk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3uxwcgngs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3imkeavms.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rnifqlho.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wpcigkpx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3hnqlknzj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3agffsyzp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ooweaqzw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3qlhswjye.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3svrcoviz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wlrbinuv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3qwhdvyzg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ukhepugk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wtaipagj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ujyommjv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fcimpyfy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3dvephcjn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3cbeidbkt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tdnevbdt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3nijkrteo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gliqnexw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3achcacgk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3qejrdyqj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mnytxfbv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3luvvbayh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3tldwcmqh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3yazaaeie.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3mlxxqpqs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3afcqmyvh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3sxdekdxj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3batuasme.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3excuxisu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vvngpxsk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3fiulwfqm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iagvwaxn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3yzdorhfw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3fctfezim.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3crebardl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3raflcdbk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kcdirmry.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3zwhrlzit.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3faybtluk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3bxeylgsh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yomloacb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3wzrycxnd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3scutnwgc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdjgzbro.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3wuwgjozz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kbogktnu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eojtleth.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xvvtzojt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qdbqgfvs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3prukyaiy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ctbnnxju.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3hcurzihd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3modtsppb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3cchlevyu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3trozqaxt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3gfpdgope.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pmmahldy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lprwuieo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3yiyagwuz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bqtyjhkx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zzzfaqea.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3mmxzbxyv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3izsahdup.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rtjnmsrn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3szxlfzab.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3anfjfaxu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zxqskrls.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xzyfrdgo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3bomexddf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wvdoutlx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3aoxamgdh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ixqjokon.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lubxuauf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kfjnvuci.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3tcggfwgf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oxyxusxb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3zryufwhd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3crqframw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3pvrlyfwh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3oyaoqvap.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3nuzlgqcv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qnbkgkce.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3eqbxduyj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ktqxlooh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3zlacffrg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3qiumqanv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3thoukzmn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hdmqzaht.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ftwpcvrq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qmmtdtch.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3otoyfuxs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jtwodcaj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3waelsujr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqzbivqp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3aoqwfban.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vewlukoj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wuicostk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uviqkgzs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3rzgaxkan.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3rbuatlbr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pdwwmfiu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oqroxopy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvtpxlcb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gtrsfson.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tephglnf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ltlxlytm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bkcprqli.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kkvrhrui.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3kkbqaqtk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3swewbmoe.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tzokodaq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3alevmfcj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hwglvadk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3wjqfalyi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3biqnuipl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jtgjqcdl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jacrhwxk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rgbfqimk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ioymvbal.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qdpcptqh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3urjoiirv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3wwmpyixc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rgbyyycp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hjmudsow.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3bkqdhxel.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3orydppob.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qivklfpl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3sytnfxsl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dqlbbfag.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3gxtfliom.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wppbqjic.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ohdqpkml.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ljntglqt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3cogychqv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3stkombea.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mhgjblye.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dorsqlcn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pbvzmqpo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3imxbnmgo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ktvqnnhe.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nkdqwaxe.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qjlqqovi.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3rkxptiaq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3kxahtoxi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3abyogykx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3nljdurei.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bzvrjktp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3hgnzwjol.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3alharvja.html


<!-- 参考信息 -->