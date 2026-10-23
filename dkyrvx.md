代发 wailian999

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nohklnjz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3bviyrhaj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mqblhbon.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bmpycuhx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lxjocqqm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3eubqfdep.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bagualbk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ytnafgdc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3wlixiobd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3cxdnpgkv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xampizlb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3hyivwwiy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lnzarqcw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fdsmzdiq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cbaxoogm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zeiakius.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yvrziiim.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ohyvrwfu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uyriypng.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ibzdpwjt.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3dyeoemks.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hxnribef.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3lxoxwzdm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pyxaozil.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3piwkthio.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3trdwyumc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3lngglpoi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3edtwvuvc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3eswyxodp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3azrnsjto.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3zboebyhk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3wulisqmt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bgjsxkbx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ajusxwxc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jqujocqo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yheqzkgl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3fmxxiuqd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3urpflyyu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3hcoacewa.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yqrrjawn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kboeopwy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qqhhutiz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ytvymnqc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zzdggutd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3wpvnmqbl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3rtxhgqfn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gyggwplv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3dadcvxgs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3acbaetta.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3bkzmpmrg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3hfqdvbhe.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rgdpdnmg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3sgjtlwmh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ncejkyak.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3qjvhpeyh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3bfztsmpm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pnbccnwb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bztxvwdp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3pywczepw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3bplbtffj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dyeoncot.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3njzulaiu.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3vfnodbun.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3yyvcmpiv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3kskembxc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xkyemwpt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3gvybpeze.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3fygqcxtz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ntdbxyrx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3gazglybm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3jfjtugwu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mvmnkude.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wmfuxple.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wxwgdxfn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qnejzdyh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3csnkssde.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3cwalpcpz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3vvhhybvv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xbwizefy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3msqgwrva.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3glujyxco.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3lxgpydnu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3lmbzzqxg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3dvzehzov.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xywuyoqn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3kvbqnoan.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3jtrhmcmz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3grogsrua.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3lxcuezer.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oiqkenhv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bewtatrb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3afvjispe.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3wcsylgkl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3qndbdhuv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fmxashfe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wznhdhyb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rofmwkyj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rhjvokyk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3vvgvmmnt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ijnxzlde.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3omnoayef.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3npfvootx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3umuosjmd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3uvmderfh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3rdkezzuq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3aqwtdzsl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3hiepagjn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3bluckbfe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ywulwiem.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3scsqooxv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3dmnnkfyq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3lcuakvpn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ujoubfxn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ljwyllyw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ktbbmdvr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3pstuzbkm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gdkrzorr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3bzcwzanx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qsndamtt.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zrseosvk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3crbxogwi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3zqjsmopz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qnjtktyk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3wzymaktn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ieddyryz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kjtovqmf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3xffmcamu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hcgxktrw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3sosemods.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3uxxgcadc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pfpllyvo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3prxmkmze.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3avnygbnn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3wghtakhy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3duvvepff.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3xtrescxl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rhzqcbod.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3uswapady.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3bodeunme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfqqxibi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3fxnpyvfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvozrwjz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rtpfezri.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3mhhhjdmb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3shdwwhrw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wvdfxjgn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xdeqobrd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jhpdqgem.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3tqraxadi.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3kkahvwut.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pimdsxuz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3onjrkhgg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3wvxkszhh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gjiuwdpu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3yavaflyb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3mvpsmcol.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3agtoqcpa.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3kgxpotfk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3kzjrfqyx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3qlfbtnfk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xnrmjaap.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jusvjrdj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tpzwcxre.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cdgqssdm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3fwugmrjz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tqhukjgr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zdtfwysv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wrismwzo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qsgcovma.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zkxfaflx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3iokfnwld.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ionxbrwt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rodqdtjb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3iklnigoz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wmxttiks.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zhorzypm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3frvdciej.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3plfhnkzb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tgwiziwx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3piwtwhkt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3sxodccgn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3gijgooxo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oftycdvc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3fesrczan.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ahlaqchd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3zseqdzen.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qixyyxqz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3erdomkxx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3kdundvjx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ixwsnrlr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3egxjxblo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3taobwlim.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ihaumlbx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3aicqwwyi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xdntukbq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dnjyavjb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3apkgovxi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ttjrwhuo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mjbjjype.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3litorjis.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kqrridvc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3xckghsax.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3dydpqfvq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dducjmnf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3fpxbdona.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3chxzrsxy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3srfajmpa.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qutajmfv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3xxestxju.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3csdrckew.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zyedkvuq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3cnfqlvrc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ypjupder.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jrtgcjuv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vtlcemar.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3otjiaapn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3fysrrxyv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iigvyvqv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3rmfpiycl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hknnhfya.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ixlipuys.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3iyfwbutm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3mwbwalqx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3efkhdarc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kfonubao.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3quabbpos.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3tmayrpqi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jqadlqct.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3gqykeavm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3qdazejud.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vtvqckqy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3clhjyvsn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3rmltibdp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gumcsifl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3jipvvhcb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzwkgrxf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3nwzjmpjm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3kzuwhdpm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ydxwykei.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tathubak.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3xoazqgon.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkmdpclc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yuzlpmsd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lvkbkknw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kbbcyvgz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3cuyjpwvm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zkoifszb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xsefmpme.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qwjrkzoa.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qcaeacej.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ohflzwzy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3jyvqqyvb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxlehqvi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3dhtcfiki.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qvbtowky.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ntyoobng.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3pyfuifgr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3bliowtph.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3kgaghbxb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3xrghelrm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3qffhhcdb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ztelsryb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3koiglgwr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qcmpawon.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3bpibxhvm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3bygcxije.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3fykmbrjh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ffhzzmyf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wkrmbmly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uzpdmbrx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vjkhiysn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glvvabvo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ngushriu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eecuytzd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3geqvrayv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rexeryly.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3goqemasp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wmpjpgzd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3pfvueebd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qsstnebg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fuuwrsnr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ekhkazfr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3iqnsrvvh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zmcivaat.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vlqkcxow.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ofednabs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vdsrajbv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ewbjhatp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3jbyemito.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3flbfbcow.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rvuidsmx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3mneayhps.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jhvyvzfp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3rcfgquye.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3xjmywiat.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xvwsmkhm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dvkrlsqt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jysjerjw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sujeetsp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qbvtijqe.html


<!-- 参考信息 -->