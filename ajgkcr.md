代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rfcxzlrc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ycelgmdn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ozpsjvte.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3siidozpf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cmyhxfwm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3labwkuvc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3sezmqrmc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3lhpgjqxn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xmrejemt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gjcjdvca.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fmhndcct.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mwatpcpv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ykgillsu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gihqgmcb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3smrgplov.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kmljkqya.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3hmfsqakf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nevpuniz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3dpyqweox.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3oxrlspic.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mfhjgaim.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nwzlyfgs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uykzxnwe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3dzljdxxp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3kbxbbsaf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3puxbgyrd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3txgcewhx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3broytmnz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3enrdmrfy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3axnnbebx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3tivpbloc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pxxsmebf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3thaludob.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3abvrunds.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ircudeii.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kkvqxggg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3khrlxyom.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3uorlngmk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ofjmbrur.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3songmppf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3oiitbtkh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3kdrxychu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xbnoazgg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jzdccilo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3euuedcom.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3hpeihwgl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3pwygwrgb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3axiujpvr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zudzmcgf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3hcurqaxm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3cthzxepl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3odszdtez.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vttywutl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bddjxbvh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3pltgtrqf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3iigggujb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wushbkdl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3hthfexyx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3khlvxvnt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3gorkrccx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dvuwsnyo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3pfnhppxs.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3tnqkazbc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rffmtumy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3eztyejnw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jhzhurlo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3lxtwnyes.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3fbkczysc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rfttadlm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fwfgtfow.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dxacpvgf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qvnbomur.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3sduoowcl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3rkqayyby.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3thojnayl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3kpryecrv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hyffbzfc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ojmrtnqk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3rkdapjda.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xpwbbytx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3lwkchmkr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bfjbxfmf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3fzyatvko.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3pwonvyqq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3cbaenqus.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xjkrlkzt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3savirglp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3iuhufbee.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3blvfinen.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hgztuhcw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3lcbckhdn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ihrarhka.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3juotkmws.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dzgbvcaj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xnfyagit.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ebengkhk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3pmhwcygl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jxkbugzt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tgxidorm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3knahppcm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3rexexjni.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3treyldzz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3aufvnhak.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3oassohyr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qozmtfhf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3iubnipbk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3cokcnmay.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jedimfeg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3nrkhduup.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pcstrpix.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3uvpeplrh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3prcagwru.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3bsorrbpt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gxubtrbp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3edbuhvhv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ayvzjwwq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3lbkfsegw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3akqrswyv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3payrbvxz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3rvqrdbci.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3leindhar.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3jakvuimf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vythfdfk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3zudtwilk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gkqctxui.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3scmramdh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ujauimug.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3pdoohdko.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3grjvbybw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qbjlvtns.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3fdmevfah.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3bbbkvclv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3mohibtzo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3davhlgoj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3fubzkvll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvyvfkxl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3cmpidwjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vomfnynp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3evxxcsbg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qgwskuoe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3wgijmqoi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ygdbgkol.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pfhxlbsp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3glxpufow.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3qtuhvfis.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qbrbjnmr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3tmmvoeks.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xvcxwghh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kradagbx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yinzqbhi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3koijrtnh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jknqxbyb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3btbwrtom.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zlanqbsl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ruzgznrg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3zhpsgoyg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3kctipslc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3yvcmehhq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3virihbgj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fimerbvb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hpadnpqn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lwzdalfy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kospzxju.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3uajxmjdw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vwcmbtei.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3gykrkuot.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ozyaidwg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3erlteklq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3btvbojck.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3aigfjbjp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3dyaygloq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3fmxzukmn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3efdcdszl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zpwlptsf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nydtshwi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ycoldnsy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3qonefvft.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3prlleeyd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jimoqxwf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3holglpfv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wputlpdz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3agmfgqfx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3gmiguybw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wnvfyxid.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3mbbszmss.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3lxktvhbc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3naizrsps.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3cytxoiyz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3yqncojsp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lpgnryhv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ablijadl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qxoimvdc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3yfdqnokq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3wruclanl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wryfromx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ncidmavx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ljxkwljs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3fzflptez.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3icdqqcrl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mflwmkka.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3bwfstbbr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mvenklic.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3pnppuwqb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3srozukri.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3lijontvo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyysoppe.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qtjmvevo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3alffmbjp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ftbxlwln.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3izcyeecv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3fojrtzlz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3artqvhkc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hvhtyvxr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fnutjtrx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3dudoznnv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uonqvgme.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3iqlilfxb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hjrtuspn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3gnxxfmsk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jvisvxyt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3svwkuxlp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ghllshvq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3daljnxgh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xrphmogc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dtimdeyp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ecsdmouz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jhgxrodl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3byyyword.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3uwupwhik.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3fhdacbst.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3xgfntlgc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3jheyehpz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bwugxcbm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3zpceehin.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3oxxbgwej.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3bdkieswi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ifnyiaxa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fubkopym.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bukvtbej.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3pxrpackl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3tylmfbqh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qwnpzdff.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zjsvrimd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3qjaouzqd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rkqofdgm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3aowsdxzk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3gmkyetbk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vheozqcu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvwzjhjt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mxanrhlq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hrbliyys.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3whqfcwdk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3yfazokdd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ujszvqnn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tpkopajs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3woryfowy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlvriffz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3rnffkvae.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pytjnvvr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wfdskdcc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qmhqnksj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3rfqbcxxf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3crtidpye.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vzjuqgti.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lbyjjzji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnyljtmm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3szkmjkoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwpgptlm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vhbefsib.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fxwjocky.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3swfsjyxd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zsocxpvk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3lcjttzcp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gultidqd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3pfmjmpaa.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3dsjmsmgo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3cubpqrpt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3alxsruql.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qvcehtxf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ykeuerhj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iyleaoqh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jxdemnqu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yemfdhqz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sdqiwelq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmdzqjdq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qcetzamr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wfyjjkpk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bkgrszjv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3lqukklyk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qqhncxre.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3afejqcsm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwvhpkpd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cjqipslm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdnrzyxt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jbvrwyme.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3boumwnpr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kmluruuz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3loudjfeu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jvbcqdpy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mupfpxsf.html


<!-- 参考信息 -->