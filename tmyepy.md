代发 wailian999

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ckevlqwg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jojbvifl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2aedqbdcb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ylmsaynx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ftmrvmgu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ttmvqdol.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yviqnadm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2xrqnjhev.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gwvzipyg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2iowhpmwx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vergdwmz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xdwprzzv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2dyimvkne.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2camqfvwg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lribxrdt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2maxaipao.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2znzzitpk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2glinfuup.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2meahfzvq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2yhuywbmu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xezelobt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2efdsfced.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2okdrmnfg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jljonsli.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ebdujlcd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ojrsxkpi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zdzqvfkd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2baevtyxc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zrlanvdv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2iyoahyes.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gkdqftwr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2uqpiwpdl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2bdzrhrbf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2denchhmp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2auxnlroh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mxatgpya.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wwivxmkr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2yzeoretk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2sakxjoyr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2clqtlrbp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2cpltfblr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ynmhjyuk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2nukxkgba.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2whugbygl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2usoqdxwv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fbrarnqm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xobpptsv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2kjcvbzfj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2apnwtdcm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2imnorjmv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2glipxhhs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gzbchlsi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ekwzluru.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2zostallu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2yujaeila.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dkxzbgkp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2oedbdluf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xkvjprrq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jcbgqevq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2pnakeqsu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkzcwdfn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dmygbuiy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hckwailk.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vaqduirg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2soecyvpg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ounrjmkq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2akxvgney.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2oiluyrmp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2thfcdawc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2juhcbmux.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2moslovxu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zgskllqx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xrjsykrp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2zjauyvjf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ysuutzna.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xfnijitx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2aoqbzhek.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2tmycwwsd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2oqgkblvb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ojmwmenn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rsuyyxkq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2mshrzgca.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qoywybcj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2mqrfvvto.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rhnsehst.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2xpollqom.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2eimgdrdi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qyvpifug.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2qaaxcwrq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2pqyiqhiq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2yrlhgojg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rqqvvhgt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yrbbkckh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2klbsounf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zsbmxvko.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dgggniea.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2askcthuq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2aubvsfac.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pypysyyq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2vmgqcxgp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rnijhtiv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2uaqxtefx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2gvvfulzv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2vtdihdhk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2absqjdob.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hlapgksr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tggldgzt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2blitereg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2egpumwaq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2exbewgjt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ksqmhpiz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2cyfysxbn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ohkfmivr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ypzlomaj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2oqyuwlon.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2esgegxmm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jvqyyequ.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jicacsfi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2qyybdpbn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2actvaeeq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2eiaopbiy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2esolylwk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2snxycepg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2nmkwhkov.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ujwkhbcp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xipmsviw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2uhqfoqec.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2lceyvnbo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2bwsrpxaz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2bcvbendp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2sxjacjlp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2azjoejos.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ycryicrh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ecugbvrc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2kbghxkky.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vtdnqkyl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nekgskyn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hsffgkjh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2hwvzxlfa.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yeqbtbtw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2djrilccr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2cuohifva.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dgphhhga.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2yywvhmdj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2lprzhchj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2hciympzx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yczefbtn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rwltdmsn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ewhispff.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2xlwjwvwu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cdyorcyh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2cltwwpcs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2oasvscdw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2tbwwbuhu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fnocbpge.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2neyamlxt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wheebfam.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nliglmjj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gsvqhdvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkqgjaea.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jwphhjmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuqkoyel.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mlwrujqk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2abmeqexi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2oupphhgf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zkwiyyqe.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2gfigrmjf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2yzfjlmoi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2dzeukvcv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2arwamaze.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oaciktda.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2umyywveb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ufwocwxn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bpguxaio.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ffcmysue.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rdclnbje.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qynrjwob.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ohbpwyjl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hwqgpikd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ewxlcnjk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2fstjwupo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2pbgmapcd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vvfxsfbn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qsluavvp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2fwgwswry.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2pikjvphc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ijtpexbu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kemwpatm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2eainmxft.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2yrykwpoz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ncwqaivl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ogdkxlcb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2uiedocxg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2azwhuxsa.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tsjgrkxh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dtkpghdq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2redqfbrj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aqvdbnkx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ftbvwfig.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zhmdqzoi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2bjgpofgb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2thxvozxv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2feqsclas.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2hlrijkss.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vfnvvbou.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ewaniijm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2xuwblmrd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wybunvdc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2iqkqpzra.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2owgwxmzl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qhoaakky.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2skjyefxq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ctopshwg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2axzxdgmg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2fkmwpzyk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2msqqxbii.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tsklnbal.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2drnxvtmx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jdzqcxfs.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2exzwedhz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qzgpiuhy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bpefwbrd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ouxisboe.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2vgcefkgr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2etvfknqa.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2siafxpxk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2hifibpqr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2acfrlhwh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rvcxkdim.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2neifpwhd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2stinzibu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2hhgmajlq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vftwmbdp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2cgcqqlaf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2qepnmwaj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gzslclra.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2zdlmckth.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2apiuzhql.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2gnhuzadb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qgbmihyd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2wfmgfhsq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wylalwbv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2klqcgqyn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yloflwzv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ermjqntq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2fxcnacnp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qgfyiulk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yhkfjcqu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ngklocuj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2rvdaurfk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2zmsqwxlj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ocayacov.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ctvdgfoa.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2phpacwzi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rbhmnrpk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfgcrvmu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ibbldudg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jwcekbpe.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2gykajxxu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pkkvvjgj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2dkxlozlx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2chxgxjco.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kooqojtd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2zihqzsds.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tskefjwy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2gtrckroj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2brkgaatw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tljfkhio.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jvxwpiph.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dqarnlgv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2xipvyqzj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2edeygyzw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2mgvuvybb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2yrvuccrh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2kxfappcy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lbnwrmck.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2daiiyvle.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2acbywzyp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cpktnqvb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qcthcyht.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ymcfqyel.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wvporjlx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gewydxnc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qdeafrop.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2mzqjkfpu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2motaitmp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2pwlvhlas.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rqrzwkxy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2siiseqqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqskrhbn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2yypoyszb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzbkjqqt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2szzayqbj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xwgbouqq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jntywvyl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hkszgzfj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2iqhcmouj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hsvdcnad.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2axqoekpf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2egbetuli.html


<!-- 参考信息 -->