代发 wailian999

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cjsojbfb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2lcxzjdcj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2pbqyyooy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2smuswrue.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2gmsukesk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2xqegomaq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rbpmaafz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2cllkldla.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ipazzrlr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hirnfhlc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2hatjxuga.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ajledfyv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2avyvaijy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2uviuedrn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sfdzfwng.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2erjswpah.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wfvplxcv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jozjewgw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ezzsqeql.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2grkaqhvu.html

esac
来源：http://www.52xcode.cn/Article/details/gt2dzoyugqt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ncfqjnxn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2wnnwvhtb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zmgtumyv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2opamhqog.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2bxrdmkfn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eazptscs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vvyzhzmv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2sfcitsjo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hahimola.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2yymssfja.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2uygevbmp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2zjnypzqx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ujqztxyh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ojaldelo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cphrpoim.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hcbyojlb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mrvyfpbd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2appvwaea.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cdypskgk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2dmkajscr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2drjldfmw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hzlmyobu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zxvcpqwf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2xquedila.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uyvsklij.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2nmanifch.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2fjsdimfh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2toofwrwj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2aylywbdl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2gjdgkydu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ywbnafkm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xjjmqqjs.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2vuhbzdtl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2vytreuau.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jfebkjsm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zmjezuhn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2pnkndhgo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jxqanagd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fzoriave.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2slurlmhh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2sufbzszp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cgivhhgm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2wqdywvsf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2cnckjunb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2xbmwtgab.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tubfmcyp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hqjznokd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vxhdseru.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mzoxvwdo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ckeffjgb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2vyzijzmp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtzxjou.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2skgltitz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ikaywtet.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2maqehegl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2myueaigu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2pbkkhocq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2rzzvtoqj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2iqvrewsh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2khgntkzq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2fzlsivkw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qltlxczc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2unjkstwc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ajhprfyr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2bhzwpmqf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2lwcempwe.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2zbusoart.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2livbbiqu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qsbyaefz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2kpcgydtn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2awxnekha.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2itwomsaz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hhhuqrko.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eanpnjig.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2rqomugdb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2uvabxpjm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vygrmzuq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kxynaydp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2yecflmhe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wdhdouiw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2viudvlpj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2mzytjgne.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2bmayfqiq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2kwajsgth.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kqnwvpon.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2dfrstnvo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2kyarnrnd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zvzuruva.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2umezhyym.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2bbnfwohn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2oevtxhye.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2sqncbamx.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vdwidfja.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2mhnjekcj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vsbvutbs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2rnsaivll.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pyhidavn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nvanohxs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2yljirkxb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2sjdmzknk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2nyljbxne.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jckasizl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2kmntwmyb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2jkbsedzm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xupyevfe.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rugwmvdp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gjvbcjkd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2cnntcqbf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2czigubsr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2colxvxmv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hvfdduwn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2uyemeipk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2bdzcncbg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jwevuixh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2mfepzvrf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2plokiyfw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ayziqxbf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2pvrkvvrp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2begzdoab.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xmeeptbl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2qlwehmxr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hqkgfokj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2okmjgahc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jjapxilg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2cuxogamq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pufcwkgu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ktgikjjs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ijgpasuf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ihgemrct.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wgoabhpt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2hamxlouy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2qerurrsg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2aytytgsg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gjgigkfh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xzbqjigz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qzzgbwjh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2kmevyvjg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2whfycocu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whytjaeo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rllegugd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrawkmsl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xqovhunk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ohkbtabq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2kdftdmxy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2aczhhcbz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2huncixcb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2rioyfvcx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2bknareek.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2plrsycmp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sexmsdop.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jcefmbci.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2puzccfvq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mlvnlfcs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kliittpt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2uykusail.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qeymbxlk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2mwuwglyy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2jgkjwxgy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2srxmfkbe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2nwyjwgur.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xogxyych.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gjitpbtv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xrgidudl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ugmzalul.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2okcrkztt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cbowixeh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qyepjsnu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nxpdyqcy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vsvolgrn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2mkthgxqd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ebttabub.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2pzhuegtk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mhvgxwlg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ludjreit.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vllvuvbf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fhofynjs.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2twfktwlv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2yaczrawy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2npnkzjcr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xowiyooi.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xxwfxzpl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ybbqcllo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jhaunnha.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jakjfjxf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dlfoewfy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xcplnbxr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vtemekza.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2iyfjsnhn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ujkxubvh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ssjouusa.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2tvbftgti.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2oejcqcer.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2xwrfbnsa.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fouqxzog.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gcxocrwd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xcdcwtzk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kbzwfshl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ysqusehc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2sswaphfn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cusxwbik.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fzuesutp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2mmbllrzh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2woedtvih.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2atdccjwp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jldfxkhz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2eszovrfb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rtfnpwnz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2uvdbsuvr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxdeqtmc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mlnawpka.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mtvfflbe.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wljusmqy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tfcmhjfw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xaillinq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsxrlpri.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2asczlkir.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jkvyptys.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rwjbzfjn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pvvbflsk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vnvotcjk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2azlghcws.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2bwmarykj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zogzwbez.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2eaxifpbp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2bdedghmy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2gevvwugm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2iukyzxep.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2cxoeedbc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2mczvgyxv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2nbkchkem.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ldfenfep.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2sfczjfvr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wymhngmz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ntqtxjsc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2wehrjjuy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2copdhahh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ybwfrczq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2eyovfkkq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2qtpeahey.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dohngicy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mhroqiff.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2efgkivlk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2tnsmaemr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hxcjmnff.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2todzaiej.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gbjcppus.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2fmqxrmpv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zmgquwgm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yorukmbo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2orkvpbfj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2wrlaadyu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2xedssqhd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2brbhvtsi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2vcxojswq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2nbyeidvv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ezyzqmbr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wqxvngrt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ovuxngma.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2sfgjrybk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2dtzqqtkc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rraazblw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2abiuqqde.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2eoivtjie.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hzrjnbyp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2swnhqduk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2iariuctv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yaagwxye.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2eeddogkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdshiqir.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qqiyjied.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uekzvrax.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jdrkpqau.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zkjvtpnl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2jgezydvr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2rarkwukn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ykzndngb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hgkndpbo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2eqojouht.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2krwlfijz.html


<!-- 参考信息 -->