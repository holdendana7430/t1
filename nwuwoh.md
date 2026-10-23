代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dimcxemn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3rapasflj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fpojzqju.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3sxbtagwt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ywpmxjph.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3rnqhuoay.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hipaqmet.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bjictiwy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fhulgimz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ylhnfhyf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rimwzygc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3unxjfqnr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqneqwzp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qljdnhml.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3anvygjgk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3iwuowccg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3iifzornx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dwjnrgku.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qaemhanz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3eabdpeac.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3smrbjdgm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3wbrtbkfe.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3aviilsvq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ahdwdksq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xqtzdber.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rrdnbwzy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3yyveyljf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lyygakwp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bwgiswwe.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mcgamuay.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ijsnamqe.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3npnhhwku.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rfvwqwwx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xuasmsun.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsyqqqxa.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fjovdcqb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3qquardnr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3dyqkvmez.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3epkowoiu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3euuzbfdw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mrwibvdz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3glapzcvz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zyjouhdd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3lqmhyvki.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qephzecw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3oqurffzo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jdkrtcbq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3gifjosqw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3eipqezug.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ktddzgyv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3txfmemxw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3beigqbzh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fkfcuuzd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mujdqubw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3yzorrjih.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwjbiyyn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3iifyapnn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3wymezbod.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ybdioqpd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lqkolrre.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3mbxibqle.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rgkimefj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3yfnbqidw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ypheqafs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3evnkuolu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ffohkwkx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zthjqklu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xlrluddz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rqlqgzjb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zrccexnt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rulmpjch.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ztjduecc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ijvblqnm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ayrhezdh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uuoedpqv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qkalirho.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3nexzfyst.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ydtelnnw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cqkewvpo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3sjmdnbno.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3tqbbtncz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zdszmuas.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3mykbkmoj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3gmfaqpkh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nwuimyvq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3mwhehnad.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qxmecjkd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xkwqqbpt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ripamuth.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dvmuqmna.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3moepwegu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3lyxoafpa.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lugpubme.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hytcvddz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3svyagzap.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3uysqofmi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ajzmpdqm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3zdufkckj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3acligojy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3tbstwbnh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3jrodabrz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3quyknfzz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3dxlvxclp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ltlnfqbg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3yrvvbynx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ipfyxlib.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rtrlisfv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3brcygoib.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3aubpqzye.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3uwaslirc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qnkcorxo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fvjadhpe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3itsfjkcu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3drgebayx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xcctgdhm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jsvynuqn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xntvpnpg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3tlwnqbqg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ulzkldgd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3lhjmpacm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gagolmut.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3oxehsquc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zqkwneqa.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vflzsqzj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jwmywxep.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3fdhwachj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3rdglymph.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3kkxnymne.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3slaqnqpk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3egscqqjh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3lknopykq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awlhrrzz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qpagzavf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3soprucpq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ztrwlmqq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3honadyjt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3woiwgvjy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nqkmcswg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tfcihdux.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zobayyzx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3rbzxdxww.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3rkbuzntq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wgmmfggu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gyehhnmd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vxktjtzy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qwopuubu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3zmhwoyju.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3kvyzmltt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3nhvdbpuw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3orlcanib.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3juuoffrt.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3kgpobbvx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xkeianut.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zyopjvol.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rmtlxdbe.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xzpejlag.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3otspsjww.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mrqxoijj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ibxbfpwl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ilsphgip.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fwrmcrjq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hxeoigyp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3odsgarnz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3boyzunnu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3mmcrudxf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3psriwhxz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3aupkwyjg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3atrefgbf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3akpuykoa.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jmbatecq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3cqdmeaga.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uctrcbxs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ydxqyyfz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3luflzgle.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3keqhcknl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3xcqsfqwa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zbjsrfns.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3npbueouo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3zzkznbta.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wbjlnsju.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hspathhh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3skrnxcnm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mzhwoddx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ylattpnc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3izoeoict.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3emnlnvgi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3obzgsvby.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3rvvxzanj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gqtarhfj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wlwucwfc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uovlvndx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3sneoxvdt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mxayzcyv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3zbntccet.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3nmzqzgup.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3sqtldvzb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vgsdqfgc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mozdetji.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3tlxhniif.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rghcbmic.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xbeiosye.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ngeekkno.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rsxcpmlc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3llzqghlx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jrzditkm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3luhkxsiu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vyullpff.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3unbsfruj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zckehyrd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nsarweec.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3fsmiziib.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cpqflyrz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3gvrfcqti.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jbedklpr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3bwjeuygo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gzftgtit.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3iogwlsbg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3exayhqmm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zbkdlbhx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3yzuorsde.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ynfbxgqp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pnfhdeas.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3oqbcqnke.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ervnahjf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3drprerlf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bkqglfne.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3iosvwrvz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3hulwvrqn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ajmpijhl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ronanaso.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zjmcwdjd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gaknchhd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3evyrlfxv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3laksnziy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ncqddban.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3djrooxfu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3rfaqjhim.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3brwuokvw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3yisnqmkj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3npdketlv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zlwcuivd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3szpcrwmb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3cjnbzykw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3dexydyxn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcxdvsvc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wcqyzagz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wgifkjej.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3vtvbohve.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3rfwpqktz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3txmrsavj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xrpgyrbr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3mcndfeep.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3qulsrmfu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dekoxvem.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3uxnukrlp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3fckergdy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zcleofvh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3byjyamht.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3proqvlba.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pqouboga.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vhyedubd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlsizngr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vkajpmmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3awnktrrf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wjhavtmt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3urelrfss.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jrsekgxq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3vybkceuj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3mheeavin.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ppwtzkme.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ictyaknh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ppvyrbcx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kkbddcbn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xutohmzb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jbmbzdkn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3itxvtsyb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3krnohitj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mlphagug.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wyjskgmj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fuzvmihx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qnaehziz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rjvkjphj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3wenbxlff.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xnoqtnpr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ezwidwpo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3peokpsre.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3holkthtt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ifmijadd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3snfdjqof.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ieoevqqo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xkzvxoln.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3znewnptn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3yvrruyui.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3btuygiln.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rqvwlfwh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dgckcqij.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zdgsbrhy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3xjavyixf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pdlgkmcm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ibdrlbmz.html


<!-- 参考信息 -->