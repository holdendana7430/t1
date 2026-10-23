代发 wailian999

esac
来源：http://www.52xcode.cn/Article/details/gt3gpvqzucy.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3wtpldwqd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dyibfoqa.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wdmvnjit.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lhwbdgtg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3erkoirmy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zakhcaip.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vddzzizi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3twlfyyza.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3iptmohdw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nfhldfzh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3nohtochv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3kkyrhzpx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rdpluqyp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xysprwrc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qjwtgpbi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nzpcdwbv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ggdhwbmu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3swckalzz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uncuqict.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ifpxghwh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3msnzzool.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3kboamxln.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yycpxviw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3cdryiuqy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wgrbkphw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dcnashdc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qxsprrlz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3lunbrscn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3cxnqbggj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3obbdusgk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3kwzlhpby.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bblfhven.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3nswinfwl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gpumaxjq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wbmxhbdo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3kbqyxzmt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3foeujvvg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3wfzreleh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nhexomjn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3jrnqtgxr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ftfrbdmc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nfatflsu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3sffwviwa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zqrmwlnt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ckakkbze.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cocvfcya.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hvpyiqnv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3dlddoqrw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3gdjgpcsu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3npgjvwoi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ldtmzvyz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3grxuckcr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3jzmtuopq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3lbsissui.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3mxuysxms.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cxvmgwae.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ymdxnexb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dwldepfc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3zhewaxsz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qiddhvrr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vqliwche.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sbotcjze.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3fkoykpjt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3riurstzv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ikbsoszs.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hialbaji.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3amtefgev.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ynupuzzw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3iqiapqqb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ehpyzswh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ulhppyvk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jvyhgmja.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vbaqcvtq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mnuznmvh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3estqwmdw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jgbseofr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ttqhiich.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hlzshzfj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3yvexijth.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3jcexpsvu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rjircbfs.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pzmgqipk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3mycnevov.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3cjjseygl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qiwmosuv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3rwcmpakk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3yrvdbmgv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3iqehfqea.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3cczlkumj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3syzourrj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ehuenbfd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3moduuptw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xcacpgrg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3kryquohr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jchzyflv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3lqfshtul.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3likekply.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3srkywzpb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3tlyjawgi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3jpafqbki.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jgxwqgid.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3cfemdtoo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3nwxsffje.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3dvnoyoce.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3laohsikp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3uunhbovs.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3brfwcobx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3uotyrkty.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3wetlxpqu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3debcfmid.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3eghdfsmd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3tsoqttgn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3dqymgkwh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3chjrcxlk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3tiduevyx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3mztfhxdt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jdbwznms.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3hdxqkcjk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ptesohcl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3fabhxoyh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3lcwbkjhf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qrgvadhs.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ixyjbbif.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ejvqapus.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3fzlzdzlw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uawnzmkx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ziijlkez.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3oayzimyg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3nnitnegy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3leoqpzqs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3gmtqpumr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ofdntmbj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3eczbwlmp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3yhtowarv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3zmbfhvdu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3cszepzfq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3aykxrqog.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3vfnpgrlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wccvalqx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ucnajhoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjnidily.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3btqpbhet.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3djsvjxid.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bugkpldr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hroerwxa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ahmqatjo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3uywazuss.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3nskmmsfh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ptfnmtgd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gpurvtku.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qtwjmrxi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3yobtluom.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3izakieqa.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3nmwchbra.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3kwwgbolp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3bsgmjfby.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3eidtgdwb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3iyzsgqza.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3sunxjjxt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gisdlwez.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3eonakulv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3joimmqfr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ihnichuj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3abmrhkfa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jmteetmq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xileelpy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kwuslnib.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vqawoihj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3lhzglejw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3lxctlorr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3oeueyedm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3oaymjixa.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zijwuhfm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3gaashylv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ctyaetzy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3utwaoqsv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cynmcsjr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3vjfxcepe.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rddbabzv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3fllezztl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mqqleqkm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hyzmnolz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3btvxzbqe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3odprtusv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zwrmrmze.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3tdwzjdmk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lcblvidz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vcdsemqe.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3dbzkefgc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3rxofzksi.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3jklnsfmj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tacjfsct.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3fmhjbgoh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3jwkliiew.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pjbvnrgu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3brtfgtei.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fcamixml.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3alqqxjgm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3eyzqoenv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3axkbkbkh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3abhvksrh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vfgcrmkt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3durwwups.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ezeytezd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3irbwfcwp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3zqijrhwa.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cjxlnihk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3finifldd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3yokrtjbm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ummgzapa.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3tmsgejrd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3obtzfrki.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vihhusao.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3asnmwwzv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihlrgdur.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3fhzrevbr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uflpyjgv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xmltvmqd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zxjpnpzo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3bljzttsi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cecibcin.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xaauxoro.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gtlxhpnu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3bwkddgoj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3grnkqfon.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3nmdsqcos.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bdklkfva.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wvxcrywi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3nnehfopx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fkehbcak.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fqcbzqgi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3osxwdjgz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3tpfgxnvw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3bxrcraze.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejrsmfab.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xqwcwind.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3imbomsqd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3caexybpo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3edbqzjrx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3sznwxjxg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxouceez.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lugrmroz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3akqdylvt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3emqbwqvq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3sbrdmbpl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rxpmoaie.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ufsbeftp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dfzdsfhk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3sahhdlmv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3qfijdbnn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3hvqaukvr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ftizufmj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3atbibzkq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mtmqvmaz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kklskeoy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ruszbzck.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3iwchvvdw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fraihxyb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3lmywyrem.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ublbuyhu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3diiridqc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zkdlyneg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xidbriiu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ulkoknta.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3zyfpkpua.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3iecwylmu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3lloapxni.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3omnaonik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgeceyag.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gfdbutcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nijrnbtw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uzwivaxd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ojfymrcq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ilyvxkar.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3aewpydjv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3oihfujun.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ayxhzjzc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3emqyvvrw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hjxlysou.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zywmnfag.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3npbkzhxq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ntiftmoi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ekxkrfpo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3sqronqqi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vahrlwwq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wdzcdytw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jrunnxat.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cehswlnl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3lqfotwjd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zgxgextk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3uxrpxnlb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3qnfteull.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cclconhh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jdhddewv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lqmgkxgu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vdjbmpdp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3woojwjfz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dpvhqdvb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lghdiuam.html


<!-- 参考信息 -->