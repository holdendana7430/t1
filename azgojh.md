代发 wailian999

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3zngojkpm.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3hbvlzlqc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jeheqiqf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jwhitqbi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nrnlrugm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vxcgnaei.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3azotaaxw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ybdiqitd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3pjskhzad.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qlxuvvjj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3gtagpwge.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3uurqpbic.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3flsyrwas.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ozkvbuxg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xqukjuxk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3txwsbflo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3usoxitcg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ibavqpty.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rjddasna.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yftjjtyi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uxqefdai.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xxomwvoc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qyzhjcdn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nkfiroao.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lquczllv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ucatbuix.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3twijqxob.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3oqewhbev.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3nxmrtrjh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3mxlwosps.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qwipnnia.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jdokyvif.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3xxdrvyza.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3lkgdbgeh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jczoluyx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3litvocun.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jytrluzb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bbrvqwol.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3gbpbzlwn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lufssswx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3vymxzhwj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uulhnezv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zjwtmuso.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ywxdakbq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3seemxhjl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ehtuelpl.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zslrqtxu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3tilzuzvv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3osssgytf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3qwzemhdh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mnazdoqv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yazciaex.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3snlxjxcc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3bjqlwdui.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3gscinrxu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ndggsacf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnutplya.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xbvfrphw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gyqynssr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ivnjzdmf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3rfpabfdy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3nupwpyyc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hgwtqzkz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fbfzemfo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mqmpzizj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3jxfodxpu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3auljqcpj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3cgeukmya.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ektrjaas.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wyjnqpuh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3hgznczgs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ezgmtpfb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3rszgbcpz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3pizqapse.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3jmfwrzjj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3lascchpr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3oxqgrzow.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3tusmspmh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3toogvoed.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3mlvbpdvx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ttqrvigm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3rlynkssf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ultbeqec.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3yxgsihxq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3txtxbcjs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3nwxkxpkp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3dqubywor.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3bmpzwedl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sdarbkqk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ltqkrmkk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uiqiavwf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3jsmrramo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3gwpisvrc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3sutigasw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tlbbrkvb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3smwcnygg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hwpewool.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3lywvonrr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zsytphoq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3sewkfvca.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3voegvyho.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3livvkinf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3argxhmdq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3gbxkmlzd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3vyhqmiko.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mwcfxmzw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3efdkrcwb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3oihuhoqw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3eqzmdokj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3kqerhkll.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xhedivii.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bzrtwaaa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ldsdboqa.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3urkvfxbh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vmrkloso.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3uzfdqoug.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ohcnolqb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3evizhwwp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zozbhxuy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3xrggsebw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3pixjjtga.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3gxgnamse.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zwihorfp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3guyrsqly.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3zmdwgnpr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cdnwfrpn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xdevlftl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3grgduvrl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3cnsxtahu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3gvfwgukr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3agycrovk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3agpytdhu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nbppruwp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3qmccybiw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3kzjljtrt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oiwfwvse.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3uqozzejc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3gxypojnl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ufuoyqhk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jmxcacdi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3bygilkzg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3grejuaxz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lmutulss.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3pznmqyrs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3rybawirb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3gcuyqnzk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3uyaakucw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3xyenfgvc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3rdzxjvwj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3kvmwpczw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ejzdzegg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ywotxlch.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3udmngdbe.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bvnurang.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hvfjkeyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omyjhpas.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qhqkdhts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfokllmx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gtdxjbjm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3cqhgpkjx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tstjhvuy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ivkxbgis.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ahwfatkx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dmpijcip.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bwqforoo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vofcemuw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dhoslxzm.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zptzpewt.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lnesbqro.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fenjqsks.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3hqstegiu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3attxwaqa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3pggigevd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hujwazdi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3zzutyrtu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ecptvvgn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3sbmbbbdm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ojkjjbgo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3eacpzhzs.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3evdupkka.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mfscgnvd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dsvxngiz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qhizmnhm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ggnwqpxw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3szzxlgqf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3mflsfhqu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3asmxjgxc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rffyrjcn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ltvljmgi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zvtqmwus.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ygogvhke.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3uqolxsty.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3xdthdxaq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wdoxnghd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3cyrufmcn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3czswrvss.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ddgvxhdm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dolggmag.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bjejqgqc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3wxdjjkpg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wtumvcyt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3enarumat.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3neorycyz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ghyawlyo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3yoirwbjo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3gsbmpuxc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3qisuurin.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3vuvysmfi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wwstpubh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pnnzllbf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3txnxrdtq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3kmgfkfdq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hovmyfyx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3tzlvcgfj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3brrmcbqe.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3srohfocu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3yneoteva.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3hlfhkcge.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3eymsmyus.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xnpzveck.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vbddokuh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3pjerjmog.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jdrrmvkx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lwjrdgha.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3nnamsgfp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqahvxak.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3obhxgmwj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ivjsuptx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3cwgdhasq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iqnyxcmn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lmsgzear.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeofolxq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vlvhtklq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iwhiggcl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xhfjinzt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ehxgvest.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3sqvhmope.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hkjredgg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3obzmcpsf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uwgtilht.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3etylqauw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3rjqeoihj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3mbdwhjod.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zyjxwwep.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vwqgolah.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pjhzybhj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3czlbpsrz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mwebevhk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3idjewvij.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jxdjfbjc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3wkghcrpk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3iwnvzctr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gbruarfy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ojrgkpie.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jvfmkdev.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oidkairo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uvyrspur.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqaqdsco.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sibiezwc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bbajbckx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ondvrwpo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3towipmhe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pcrxktdc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3hvhzqzrc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3owueutzl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3nkolxhdo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fawffwep.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fagabcds.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3yghitmrd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rykbquzy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3oispsbom.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3trcucnas.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tsmpbdyz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3xirgmzbn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3mtapiefd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3zdzmbwxo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3aupdfvjk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jcczglwm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3havcqblg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3unagptgf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ycvifwzi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dabobkra.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lzhjbibq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3vpzhvtni.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cxryxxft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnrzagdc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vviqtthd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwlvlnrq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qgddyigt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xcamoted.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3phsbcqnx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3evbtkljg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jmdijouc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tuybqjiq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xrmmknzb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3txzsvkkb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fegtlsym.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fpyrmsgl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ehxzfwhd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tohmdmbb.html


<!-- 参考信息 -->