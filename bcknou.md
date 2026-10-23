代发 wailian999

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3uvufsshz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3czddeorj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3cakvkyph.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3eggivixa.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3lprrgjuv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ywufcipb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nadybcez.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ehcitzax.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rglixwck.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3bmhslzmm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ecsgomlj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pwgziwnj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3xnxbfvly.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3umyyplwy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3azuvdjbh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jcsiwpix.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3hgmbxwbw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3jotzalvn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3emjnuvzq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xdvmpzms.html

esac
来源：http://www.52xcode.cn/Article/details/gt3wvvqvpqd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3gjgvjjdw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3bgoqwefx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qleagorj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jlhkwvjm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3fvpozryg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3muyirloo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vkxhloqh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lcfcttdd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tuqwscsa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dpmdtkde.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ucuyqcdf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3aforvald.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3afrukags.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wianpnnx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zryetdsg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3adoitlbs.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qfbdltti.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ckftqfat.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ruskhnax.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3bxqligzu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bfosysxu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3volpalhl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cesxfxdg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3hlcswqwi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qtfvpans.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3skovoumo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3anwvtobm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3crwwevgb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3xpbcccau.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3lpwwdnan.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3rctxzanr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3doddxwho.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3fjkvbfho.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bohsxrgq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mclgutvl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3cufhalne.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3krcvqhks.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3avocgjmp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3bzlnkzxi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtklxbys.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3hueewlmk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3svnxcmuc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ewaulobv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3nddxailo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3glcctkab.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rmvmddiz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jzzeookt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3lvqxqjvp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3zlhnyicb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3thnoolxw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3hbazgojs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3mvcteymo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qiyvswph.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3dvjroyek.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jfgfiqpr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ecgfyora.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lmpeosot.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3noacbvjh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xodtbtio.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3aptamauq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3cclnkzjy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3akuxdxjm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3nugelkiz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uyjlpymc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gpvmnvgu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3pvuriuqw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3jsolvyli.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3tlzexgfc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3aqyqbkbo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zqodjpbd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3tqbbcfja.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tkibjkhq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3raiswfxk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mcerstkv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qpztureu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pqxdygkh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3bfjohutq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uyfhnxcs.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3wfrjaehw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3nraptzlz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3vawlagnc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3vgdnndjk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qjmhlqao.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3dflqorrz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ouwkpnkm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cpbomfeg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3mhoausln.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ytyfmphk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wlgzndjv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xtcvbuec.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ivdhkitg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3bqhufbzt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3lpdmzqwe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3tddczpak.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cdnvbuvz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3tkouqwyw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xzsszazo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3revyxvpg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wurplrym.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3nbwlfyyh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3lsvzhzns.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3supsncdz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fjyukuhe.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3viqlcqsn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3dhccxovj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3buvoizuf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3nunrtyac.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ludgdatb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3lsczxjjt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3bzjgdhqd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3lboscboa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wqannera.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3gemamjvz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3sdnoeylv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3lvltuzbq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3trlnxmnp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3uijabixa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ispebmdf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qhjevrdm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wevcctbj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3axpfmgug.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pvahyfdt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3hanvvrdh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3eoxbvijw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rgttxqcs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3hbefijyh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3numlkmwg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3rpxvtrmi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3liucflca.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gghblmuz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xrfwdyec.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3tsbgjqhp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3kykyoafk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3qzqwyntu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3guumhloj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mtjifejd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3uqdanoho.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mwwdzykl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkuvavxp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3pilxizao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kaggqmdd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fwaklakc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ixpzvrss.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryqlspua.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hrshqium.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3zkrydiyj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3hvgugium.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3otdcnypz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3bkjuxvle.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3akrkyogk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3obdjtkda.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3pawapmzr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yxvqxxod.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3uebqslym.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3gzbxuduf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ehivhgdi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3hxyhvyes.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3eqcekjim.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xnnanecn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gzryexsv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3bpawfqsl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yiexuujx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nzfwiwoe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3gufvkzjq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3iuipjisu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rnxrfleu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3grwgohjz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3esmsfmub.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3isaawlje.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3epedkkng.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vxgcdggn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3iguavnvy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3elcmfwpi.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3nclqzfok.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3avvnnajd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3icluamia.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zzmkyspu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mrgswrrw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qkwekdfw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3pcnyqkhq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3onixmklw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3saxbzwvp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3qaarvyuv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jfemwait.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3stftsmvn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xbuhuvgv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vfgmuatl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3xxhngkdy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3kndlsuoa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3otpkcoyi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3mydgmagk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vradidbm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3poxvfage.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3oeyqcxze.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vpddbehz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3tiedtsbl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3krmaabcv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dvtjqnmg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ovulawua.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qjelaycq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3juirwviy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3utnbojkn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xfhiitks.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3kwwkhqmk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qmybeqsk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3veufkqef.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lwefxlux.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qztuweui.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3votnpvwl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3lqtnvjna.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3smulgrpw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kanfqwlr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3frtldtjh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3hxqwotxc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ryytotnf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hsdbejcf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jdovfalg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kvljmykx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tswhhwjg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3yzlshpmu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xhtalwdc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3yxbrqfcn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jwzysqzo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3gwlkknbc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vduzfkuj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xnwvuzbs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3nfiwfpmx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wjqikytz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xcnnqgbl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3wktacvum.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3kvytznzi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3umjjjwtl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3deqmnjke.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3apusasnj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwsdetiz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3uvpzykcx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qldysibb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3hdbhrdez.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3qanyorea.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ljhudofq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3pjlmeyuw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qmsdmzst.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ylqoqmvf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qoimzykp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gtvoiyxn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3okobotia.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ylmobulx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pauhrppr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ffxbbuch.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3nshoassz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3aqjhlayo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nvwealnm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ahqbwiki.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3qljpxswy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rzekfbxw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3pibfjqmk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jqqmfvzq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ybdrrohr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ggbkahaw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppmskviy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tumaroth.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3jxtwvtfq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3emwkstco.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3asbfbuyo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3nqckzxxt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3qghklvzq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mdlpxwza.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hawmhmjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpyugjbc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3omgfbatd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruyodmiw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hrfklqug.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sfkadkfd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qwkpxgtr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3fvvvrbrd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kkrsoyfy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ctfansco.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bzhakvqo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3tqkrwdwh.html


<!-- 参考信息 -->