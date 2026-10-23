代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3slyegjax.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3jwecmdgb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3evcxkqkc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3gpliifmo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fkdstvuu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wehivoin.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3kdbtalyu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3onnmwgoq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mvjjcruu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dnenzuoq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3vsfghjnn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3aihqhzfp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3bavivnza.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3szykleco.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zzoudtmw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pordxcyk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lwlblyny.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rikynuak.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3aingzonl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hqyjkbqc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3irskxjfd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ddqmmpve.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3oacwvwvr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xeyvulcs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3usxbkedm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3provmjar.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3jowkvlhx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3orppidnl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3gxnrqmff.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3kcxcnswa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3muiqfsfc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bycugrfa.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zulqdysw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3dxmgnsno.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pakgoqad.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3rpdrzioe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3nsmdiawv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3vhbzcdzv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zgqjivlf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wvuxuemk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3uablpydp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3sifdmcha.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vjrxxyir.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3lbhgqxfk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3eynzbmdn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3yqryypcy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3mbmhylcp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3aowyhbte.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lvosffmm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3zefzilmj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zabsfofw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hzqfvite.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tqkptlpx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3botqzxnh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ultabfzn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3dwiaerux.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3biaqfkwo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jvfwzrcm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wlcglxhd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3vhmosmva.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ohxqyxqw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3thnfxosd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3plplmaqe.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ogwnqrpl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3twejhvph.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3rgndbamn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fxrzemcy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3hriblpmf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3yaicvfoe.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3httouqvx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xhlrwfxp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3fttkzyao.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3fwrluhdr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ykhaedsi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fykexgdw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3xpkwtxmo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3coazuuxb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3razmkecg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rcoxmjta.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3bfutvjui.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3wxlcvcrh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hplhocey.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3htvibmhy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3wvbvundb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mgylywbx.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3omylahik.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3sgzvzrwi.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nwhjhyeh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3jwngmasb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jyuqvvsf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3yxdkwqyr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3nxepkfcl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lkzcdlvn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3nkbbnnij.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3uquhlotk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3pgznowmk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3tpdjdjdy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3xhamnjjk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3xoigdhew.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vuznmxzn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3znrhysci.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3chkmszso.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3lyexfgwi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3shrhcdyd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3czwbsylk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rbqlfvbo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3urhxcdkl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ziwheerb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3umwzmslc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ysaaqtiw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3uybkjulo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qhkpmymn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bpbkqkvu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3hizbzbyo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gntstxtd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ntykkntn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3smtqpolc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3chyogzxj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bakmcivo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3gfjczmcv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3sjbhsszd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3sfxjkhqg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dbnnrvkb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3rkffkpno.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3tgcdnren.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3gdhfybvl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3cxmyirac.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3rbjxytkt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ojmvflbn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3nhglgaam.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3orpayznq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcjjvnud.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bkrpqeru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmjlqtef.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lsicozrk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ryiudvnl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3eykkhnbj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ssdlvdhi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3vzdlwdju.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ryydgcwp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jivsqfid.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jzmwuhke.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nbifduua.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mbrhpxpw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jubxcorg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3aycqachj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3vjwawjmx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3leaeesyk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vrsuhmeh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3shzlemam.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mpwdgbih.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dzdiemux.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3gkjgosvn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3maeoklif.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ribmrgtq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pwutodhw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3zyrdzxbo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vmrsdzhw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3upnccroh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsqwjduz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mqqwuuzf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vvmhrusu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3glhwcjmp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mkmhyekx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3eqvuring.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3emhzjxfr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pxgzrbwm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rmznrzeo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xknmzgau.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ehnzplhy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ycdpffuh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3aviyjekp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3owmxnczs.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fnnktqbf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rdtlhbmg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ghxyhpdh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dybsxhwh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3vlmwmjwp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3cqwfgiqg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3scimpdwi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zwypfzvp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vlhwtqfa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jmdbbjwy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3dzldojwd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bolfnetd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kshlvsjd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vjzpkptk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3gvvqyevi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mwcyaxfn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qsmgsbat.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eimmoiau.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3bokwcknx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nmjcunyi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3cchykmqo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3cbkrfjvs.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3bdgmgjhh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3stobzwxl.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3lrmfcekd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3nfgwueps.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3puarnhfa.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3hcsidwkg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3vtgzpmhp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nxtlknlx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ashovuxx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qwpxqrnz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wipxopol.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vxlomigc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hgjyxawd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bbdkzdhc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fuilktmr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3qjcnrtvo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3twyrbdld.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3pcwwffyk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3povbndzb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dteyudod.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zyijkyyr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3nsiitlol.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wcnxcwwy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3tilkoriq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3fctojxva.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ahuieovh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qvrkiwce.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3actekcbj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3uiqsuhrh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wectebgj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nhwmfqqs.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vpxaeekj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3niiepors.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3siekeypa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3yohjmyed.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ezaarjav.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3mpctepxn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3inkalgxb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3undogvqt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hxtrcuzs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3fvegvsnm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cpnocjac.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jrimmfbm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qfommqcx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3yvykgfig.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pklzzqwk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ukqmgjij.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3sofhtshb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3qbivujru.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynocaust.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3gabtdegy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wivmckss.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qhmpqsle.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3whpwezbq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wdisqdql.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wzahqqjt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zqkjndbz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fgmxspac.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3aiklojoi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lgjpjgtp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jucpslmi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3qpsebwhs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xjuttbbr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zdtglckx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hfddekii.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qftflrhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvlxupwz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3shkibnsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knyfbbmm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iwwkrqht.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ydhuvovn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ujufamyp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rolmafew.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ywfhokyt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ejazopst.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ylguqthk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3zlyulzoq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3htzwgqel.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3uleuxmsb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vyvvmvoo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kqggugme.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jtbidjrs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lxmjaifx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3usjhxnvr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3okopdhyj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xmqfyqfj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3cwvisafb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tgvebsrk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zaomywhc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3mwcatljv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hurzhvrt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3nitftlwo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rvgdyibl.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3nwxsssqe.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rkdvbriq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3iuufgbuv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tzorimtk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hhdwyxyo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3brzatiur.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gjaxbbst.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cprjsjou.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3dmwrxivs.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cugnpdiw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3khrounzy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ppuuwrje.html


<!-- 参考信息 -->