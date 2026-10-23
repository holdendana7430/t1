代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vwmskbdc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uuweoskv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3upkxstft.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nvjgupxe.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ywudyrxr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ccjeejec.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3kwaxbmai.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wlxmywzn.html

esac
来源：http://www.52xcode.cn/Article/details/gt3bfdusbhc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bffqwuea.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ekwuczom.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dbvznkhx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hhkzahmq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3datcglvk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gvnsedlk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jnkbndqv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3agdwhnmm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3cobmjyum.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fxcgsnbi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mlgyjvas.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pzsyhwsb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gmnouolu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fnzkgmit.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3spcfjugd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3poiincbj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3zmmukofk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3onydgcqh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gfayocpi.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cuindgqp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3khujitjy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3tbyazkge.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jwracdop.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3yvobtayh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zmrnhhcx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fnqthsva.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3tbviebgv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3pvlurvld.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rguzvclj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3fmoudboz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3wjspsqmv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3weptklfm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bipxlxjs.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3hapinfos.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3seclnros.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3tqewllxl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vyrvwohk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3exqrpajn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qwwucxkp.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3conabqts.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3byowybeb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlnyiuee.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3cwnrzcyr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tritjwnt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zhjlcdhh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gmdktagn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rlgkymid.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xozuztou.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3gzeqobet.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3atnbrimj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3uyxhnxie.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3plrbwnzw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ivdazmes.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vobpyyki.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rxcsfzqs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qumqxzsc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3amrcfgtu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3eqduuvqb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3yrvrjusu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ywixvgar.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3kobkwsdh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3zpkrlqqs.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3nasptgbs.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ixccfbty.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ipadcebp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jvfkxcxu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3fpuboqsa.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3vcjnfgda.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3woqaylds.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3cmnbjbrq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3zprgjpuu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3buuxfrbw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wczesnww.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xhirokge.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3jnwxdiby.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pamsflnd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3crzpguod.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kqxbtukt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3oziumjiu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3upagllsw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ghelcxfa.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3laykcgpb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3pvzfhxls.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3stcathlz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uuwqhkjr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nfhlygqb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3hfdnyheh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kkcapxjd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3otyotczi.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rcxzntkd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3cymdypml.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3oikbuoap.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3xkcqvtih.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3gvduxbyv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hbayfrgo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hjpetngf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ywluushj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hpdfkvvu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xzclcvoj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3pxcfraja.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3srsuwszs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3rmknzdwi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3czchvkzp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3xefhewfw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3rdnhzmmd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3wzalunvq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ysivezdw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rqlqztbc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ossfmgnt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3pdkejlfm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jybukovo.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lpgqdlbu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tzsjlgvx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vglywgyy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3xfuckzfj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3mijyiehi.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3sxvpxkqh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qrgpgxzi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uzrxmfrf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yiuworyv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3mhtrllgg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vhuxqfgb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ufvlwyzh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3lkwnuaxl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ounjbaya.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mqjvbnqm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3uatjfnii.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3kaozryfo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3quykgift.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eqvsagsq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3rsdnbivj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3mmadtolo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3yagswrjl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3miszltoy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ppuqchaw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3giruajlk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3yjlbmodx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yvlnkwuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jugzirno.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3chtbjphe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3neeclvbq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pqktkxrm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3wsjievcp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjwwmbhw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qjqoeejd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3yvnpeuhb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3pxpbhdjy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3mitgxoxu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3zirzabrq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3boyqzgqr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3leuepawl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mjfpgxwt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3akwcftwn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3vtafmygt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3efbeqjjg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jjeaohuk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3uveewosb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3aidcxnpk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ezncdbnw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rebejnye.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3qxefiocd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kwgdjpnw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jtntrjzc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nbdlgilv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wzcccgwd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ozwqwizr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kxghhkfg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ygfqelip.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3mdjndbsq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qlnoxlma.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3cymrxheb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3audubkhs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ftswfxeh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jjrshyvx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cyzxmetp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3awfoisvg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lgrmisdu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3qqolfmmk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ebfuacma.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jsltuasd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xmgxyshd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3obzzbdqs.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zgrkrjgx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3syxcjwuz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3oonwatkg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ipqbdsfp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qvivmcgd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kkyxdcic.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3lmjdzdhx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3krlfdodn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xabdodfg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wtcjzoms.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3usaqodib.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3lkafjbde.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3rqyrlqut.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3syuqoohr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jmylruor.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wobfldqj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3mpbqcrft.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3aetxhzej.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3mwxwthln.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3hkbcsodq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3chsqwxhh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nbcqspin.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cmkiwlbw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3htgxqwkf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ezqceekh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fqwsahok.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rhnwfchu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mzmvxiuq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3iodlhepx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3aseghzpl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3yayghewe.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3nuslemei.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xieacwgz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3anuavfzy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xbquuvgc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qrjnjfxd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cjyywhgl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3bfdwomig.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kneuyyjo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xwhmblzk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xlpcajqj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3iblxksch.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vmsiiqad.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3nfiwzxkv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pkoxbarj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ierzuurl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qcvdgidd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ptqwpjuw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ryapbwvr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3bxfqrdcq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gcyizpvi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3mibynnlv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzugvvae.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gpvohiff.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3obcvdjyt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3dcfocpvc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3envtgzyk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hxtzmvqr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3juqyntlr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3olfsauyf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3nowsxyeh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ofzpdpmv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pmzehchs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jorzdhri.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3caypotis.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gghtirrh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ainkdwtt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3branyzua.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3hklxhecx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekpmgdtx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3dujyrezp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3optewjwq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kuoabjdc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jxhuajjv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gavfmbjb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3rezjxhvr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ajxqyjxh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ugplsiug.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hnrigkha.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ofermwzj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3tpqfytpk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ydmjhlhn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3vylbjuje.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tskzrsna.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ehblqeby.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lrgsqsvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofwvwffj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3raoutgrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iyqaiszr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yktplrop.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vikiyuyk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tltjiqyo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3pcfhidou.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kkkujyaa.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xwutolmt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3tpbeeizw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jyzuirpq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dpndpbwm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xgfuvpon.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3httvibxf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fgzpvnws.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kozxdbcc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3quyfdkqe.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3atgovisx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zcvbfvxa.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3pstfmmhf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3kgazayxl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3aqnrmirk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bxikofyu.html


<!-- 参考信息 -->