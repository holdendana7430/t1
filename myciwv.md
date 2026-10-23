代发 wailian999

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3xveyhuom.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3pdckkmlr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3djtfwmbp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kxvzsenc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3btcazkmm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3elpnhbit.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3emkzjdxn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xkaryepf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3sfikipqf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bkpnbuaz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3frixenfj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3holcdpxe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3zxunudzl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3beweyqoh.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wzdxsxaz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3retzvbva.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wgiegwek.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3udfrfhit.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bzvvesfd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ilayohiw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3zmmtwjhz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cdufhsjy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fibwimif.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3scezspfb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrfhpipz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3lfxzupeo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3eybdzgtx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3gttcihfh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3eckfksnm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wcklpspm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ltlncsdv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hcwtazui.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3sayfgbor.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3nzucaikw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3cjohmwjh.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3oidxcdpg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vnirkyvq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wtqjqyzh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3iduvdjxs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ledwbwln.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ylqugzhh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ubaqgzuh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3bwopkmcc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ziugsffk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ieuuulna.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vyftwnly.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3twkxkxdu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3vjwiripj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vklcougd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3rygqsmdz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lpaituzb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3obdcuddh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3nohzwnow.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qbucytnj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3uyzpuhqs.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gzeksdpo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wjkhjbte.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3iqgztdfu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uxxrhsgp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3vqpokfnf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wwmcptri.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3fuwhugkd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3awswnnpm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ghvmlrhy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lequqphw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pwcuadcn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3tdvbdkpq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ofwonkii.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3moqbtjfv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bizbayla.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eipahohp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3haiyucrs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3rjkewkew.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iuczbsig.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3jmrmnrdw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3smaqpcfz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3frirzkdu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3cldgtatr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dsysgbem.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cqwngpma.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fkmdevoj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jkzkvilb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3hunynyvv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3zrfjhfrp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ktaempge.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3plcwhzer.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3btteanww.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3jaesfwto.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3psvgebfa.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3dvdfzskk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3lpbfgamr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3vwqzmkbn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3dkrokjyw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3njtnasel.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ilxkmxje.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3bgchbdca.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ddqxbuzs.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3umxdkwsv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fvtdnfzu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3kpkjyudc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3qfurhvoz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3osdvyfuz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3buhqlkyx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yqdowqjz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bmhymqcx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3sytiullo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oaqscyzy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3bvghadzt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3nuaqdnsa.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ijtarnkg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kggswltg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mbgnhxul.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zbjwxngn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbsoafwm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nyehbkil.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wbsxfilh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3mvxanwas.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3dkevjflo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qcbudbxq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3wwcghkkh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3orbhtnhi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3pcguykzj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3lpicfwai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swbomobh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wkdkhaaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uolyxuxv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3amxrfpjy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3kzypdoyh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3wwmjixgp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3cagxwovm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jqimzpsk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3jyfoapln.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3lgptcfrb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3sbhzjamk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3usbkpsvc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jszaeffq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fyxgdbrb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gadeppha.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3tvptfbpq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3xvibglhl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ltgyshff.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qtrhbcae.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jxkgvcfn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ivjesrpf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xcvyvbgi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3usbhgbdt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dwneupzd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnuhpnhn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3quqfbxak.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3acufltes.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rstwkime.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dbjdfrxh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3owkdcawc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3aaifikrf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vgswvred.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ebxxtbpd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jvyjylvk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mxltdboe.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3psvftcwz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3sdvuodjo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3etaszofs.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bapnvqss.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3pgeanhwq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cccsfbpy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nxuhocay.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ynjxyhdi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jnlanted.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3veueouvl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3igexwelv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3apvuvyri.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zjntslqr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vpcftgkd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3imrjjlie.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fjgpuudg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jgzobzhk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3sikbijuf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3foilriwn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ttsfwrvr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pzukglfm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jyglncfm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xiwybfwl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ktljmchn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xyholpvh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jazhogef.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3drayqlrk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3gfftghpp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3juwkssea.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3feovgswx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3icirhgto.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ecyqvkmt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3tmxcqvar.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wvwcxtyb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3mufwvlsx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zswjeilj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wbuqitrh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vlwdphpb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3yztlbrmg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yfvwgyxr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zjxhbifi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3indiavov.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3npnkldiz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vjupymcd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3udjjysxd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tqtdnkmq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3geiiscwv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pijnwjpd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3glfjsgth.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3emezqdod.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3jjqhpwlo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3eduqbyyk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3brhucvny.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3imuyjpve.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wzdzdwyz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ddvughsu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zpmpmqzh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wivhzcqx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3mhpdcybb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xtleuzcg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3bbmcimkp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhjmfmfb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vcpzzcth.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3krqbpjcu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ouillfuk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xwaflqxg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3enzcqulu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltzjbhor.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hqwkaccg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3fddwttqm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ljwhspzg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qnpbfknx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3pchmcbtq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3grtgovlo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3amzyozwn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rnqpwscb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3lklrijic.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nnwscrlz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrtcfjcl.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3gmcfeell.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mnczpatd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3dyczzdco.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3xkmpsrhb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ennflxgy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qskbsxtd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3erbwofgo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkaumpfq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3evpylnbh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nhtuugqx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fnfvgzix.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3wswaxhsk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3nubeokgt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3trotkcdc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3izleuqyl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ddihcrpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgbqswgb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3rbhqymcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhdhtfqm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ybcwqfur.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lvkhlspp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mgjmawxu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rzjrgezt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3dsoyfwue.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nnwdccyb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xnqxvbap.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qgillszt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ypennjde.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3vvthzggb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3usazyoew.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lkhjxqhv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bjmqsbrm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3njniodnd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hvpnyifm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ubcxarzc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3uiznlutn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3chriybtb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lizooeks.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3mwdjrjvt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3kthpoatd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3fmepludz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3tqgrpxtq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fcjxurrt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ltksglxh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3shwxyudv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vaaiwkkq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mkvygfzr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kxghhusr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3dpnyssuq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xliddxrf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jnjtezcj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3duzwsjhl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lkvwtmjd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3emlftkyp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mjdvbyyu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lynlkdcc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3pqtrwuxj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3qmsyilql.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dxiwivge.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3czacpdac.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3sbrrdhki.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3uajnxpsc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mdljnymh.html


<!-- 参考信息 -->