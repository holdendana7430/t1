代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gydtfwnoy.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobtfynqe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gtdfzoeco.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqofgzudo.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/geaomxcxq.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcchcqidl.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcsgbyqh.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gnpbbnyjp.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gftzgxpxp.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/grlzrnkdf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gisvdwmst.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gbexefpcb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcpzzgax.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/geionfozm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtamsvhtd.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcpbfaos.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/guwvqxmfw.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxijoyajg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujcjzxmp.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdmwrhom.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghgjbmxde.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjpoxwpn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcronioqw.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhtfhkzs.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gpevlebzz.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljtoafef.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/grogwzbgt.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlurrcja.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/guociievn.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gxuzixskj.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtftixmnk.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gtzgmwujk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvwkdrlt.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrlrufva.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gupsjsbqu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/guezezmmi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxnuihidw.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycsldxmj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhpjlstg.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gxeezjppe.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcrcnpxt.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gchdihnbi.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/geknsqaev.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/goaqyqvav.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkhwzjlf.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gjtegjkfq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/ghqklijvu.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyvrunxh.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbxiobtv.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gnesoocrc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grqzjcdql.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegsjipyu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/ghapwxenm.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/ghjfakqpo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gqrcwxcxu.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbkirzbk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gymbioyzb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gggpaaihn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gshewqvak.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gwmcxwkzv.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/giyuqgwcs.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gcwufdrdm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gamziglwq.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/glsvozdwl.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeuykyjo.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/grqvjpagy.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gizxjwyyr.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvadewws.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocmpjbgt.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwkbajtm.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnunuwrub.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzczvogmm.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gzpdpiugu.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffosvtdv.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiogtygz.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfagxyhh.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnefgtso.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gjuajymgb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiiglzvi.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehkffpgj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gojeewire.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gstdemlug.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gefafotov.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gdvhieefm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/ghwuxzyog.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnpdrzxq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcniqelhu.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/ghfkdshfl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gergxldxw.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gvcokfidt.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gymzgojor.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmzzrdnj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gyxkqcrvo.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxemcrjrp.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzcqwixdz.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulnwbocg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/ggbrffvnt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkcoimul.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwvgrrwv.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gzhmjjtss.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/glssivrga.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqrnvpks.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gqepdumfv.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsfveydc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gvggmixns.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gwzazqaxl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakvdzpza.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gwwjbozlb.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gnhhgxwnc.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsamckbic.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gvyvtfyjm.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gocgzxgqb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gmxpkhxfp.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gshmyxebk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlkehfrs.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/groybkpjg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gusdtjcmp.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvawqkian.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjojrfmc.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gukhfascy.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuyiomvf.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsmbsctj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxkswswz.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gejkudddc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/giebhwawg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnyjocgk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxykfdlk.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gwtnboquu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnowvpybu.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gqfqhhdcc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/goqxgvtmx.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gbnkphulo.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflpvmexv.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyvqswsx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjomujdus.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsmxlslym.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgoooaqe.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruvydfhz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gbonzawwq.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gqccidpwb.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gklnschpx.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gxgqbblxu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmqvkokcx.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gmxnvmyvk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruzrtqed.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcqoudeg.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvmmvmnt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmglxniht.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcrfyqxy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gciyydinm.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gvsginzhc.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gwdlmumbx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdnnrjrrf.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/grjzfmicx.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbybtfcpi.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/ghzbfkloe.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gmrtruxmc.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzglpapi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaktbveb.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ggasjareo.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbqzvngny.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/grgwxhbur.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqllulry.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gdstkoqbt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkfztvop.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gzarpcxxq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbegnqgc.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gajagxyut.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkyimzhe.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/grnqhrgbx.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gcjyiunhy.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gozzhuxez.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/guudjcjmq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtwftnek.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvbjdiqo.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/giswqhdkt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gphhpvuid.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzuaybes.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/giniwlhca.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gtxxbyatl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gifmofvkx.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhrzlvuj.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gefryancj.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gqctrxvsh.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtwzvovg.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gayuqmvpr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeniwfqe.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhutnwrc.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgfshmbb.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqcxaokl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgoxixkn.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwsydchw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawsiunfy.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gjjywojxs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gntglzaxk.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/glvvijnan.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gqywmphaj.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/goyhfontq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrgtkrmz.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gcksouqfq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnhmjlpd.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gpdzprjyz.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gigxidspy.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjzgvvca.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeesyffq.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gchwnqsaz.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gcreaiikb.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gowghbrxt.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/glhojvknm.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwolzbche.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gccuncpfg.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gzyapniim.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gjexdgsty.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqrklqbg.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvhxislc.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gptcpdeip.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhimrctp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkcqhnvw.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gmqccpxmx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkzarpit.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gebkeqltl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvxuuhyv.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gqxjaejrw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaidvkeis.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwrneatx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gbmrkvewl.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gwlbuagrc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatiyzqcs.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gccodtora.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gdsgtmkyy.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqilnjqow.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedgcrbiu.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gobouqtla.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwqoxvic.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gnmjrybzy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gseazsitm.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgnbvdeb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojuqxbhy.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpabkkzp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsoxaohc.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gdahmgppf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gquveblpa.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gwkmdtdpe.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gckynsyia.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzpvajxr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqmczkho.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gfejzgyym.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gykmyokag.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gcfghtyoq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfojujoy.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuiqjpoa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwqemiao.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/grxptowzr.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbzqhqlsv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqicenoa.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gwrqxksjc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhabrxnh.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gigxbdimm.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guskwbbvj.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gfcrxjlct.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuohyslv.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/ggbolcqrj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gvfuwwfxb.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsofywlxh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gqdfmjupk.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gysefexim.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gffykczlp.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeysldhm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjygruhpw.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglizdivq.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcqqiwnc.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gyezfcclz.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyoroczz.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gjecnfdow.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkfgbyze.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsbvazrk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygdxlajp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqikbawcv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfdqllzi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqplnorw.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/goqhbiffj.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gugrryqjb.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvstzfvnw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gzfrrssic.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsjqnlwm.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdydhsit.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gihwyyzko.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeokgkwr.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gnfryxeli.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/ggklofeno.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gmybzweiy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfghhfezq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gyexuxdvz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnrfnens.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwrbhouv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuhvypok.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjteprps.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtdcdrek.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gktoxeihr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsjkoxrs.sHtML


<!-- 参考信息 -->