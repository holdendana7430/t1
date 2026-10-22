代发 wailian999

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ntynroee.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2mcarpqdy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2uhheujzz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2bfaplnfj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2uizebvcd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vhrwvmed.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ssawofoq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2qzjvdwbo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2erevkalz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2gkfkfnrw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ngqlstwh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2wumdsuqq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vmslkyuz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vdjqbvtn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ynandjyn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2aqjyxngr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2balprryo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gsjyqajl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cbumydlx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2lvdqyuts.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mrukvskx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rglladsw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wnnxnopd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2fadknhiv.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zobbtyjg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ibnhkfid.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2melwpaai.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nncyhgfn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2brmgstgo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2onsyshik.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yknyxgbt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fnixtyum.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2bajpywin.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ezmyetcm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kyjkeggq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2tpbnuimj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2bzkyozdh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2rchmfcxs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tzbonfpo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ehcsfwkd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mmahrchx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tcvhmihy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2usjwtqtj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vkcfcafm.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2dndqjnwj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zyokvlzu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2lmjxaplr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cawcwfmg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2otuopbur.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2chmmmryh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tcddaezz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2bxudqpoy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lxcwmdco.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2srkbtiae.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2zmcovrjt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2loznmjmt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nnsvxaso.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2zxhrtamd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hyrmsvbd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xjenkckf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2dblxwlhb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pbjsodie.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2apkzvyyc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vtomimjn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ihrvpxwi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dqasezid.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujjneaxq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2frmgpkgo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hlvrygdw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2qrmmofwk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qnuscral.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2vgqglbgk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2msuvxivs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2cgvioxcf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ghlyaviw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2htgymzch.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ppzzflfu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2pmraeezl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2kbssjvfo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2kymnxfgk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lsnekzee.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ebuxtdit.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ridyfjpf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2qlmgnwji.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aycnxrme.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2vxipvqss.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kjquhntb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vahbxqyw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vxvzmdxx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2lqxloizx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2pbtfwech.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2kmanferq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hiditqql.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fbtagjxu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ukysnqqq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2yhjnddbj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yiuuxack.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qerdmgfv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yivsscun.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xdjdxbkx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2txdgtngd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2uqqymvvp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ireilgao.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ylwjtfga.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2knqfocsv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2exhxtsdb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dghfznmc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2prmuaaka.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2jljmfgis.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zgmdkpyg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2bfbqfgpv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2zvbvarti.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2rndlcjwc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2pmhqtjap.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2kbbpwtkc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2oeofbmls.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2xgmofpkt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2sohppsqu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hfnqxxez.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lkjqoztf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jlihldgy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bhnprgew.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2dfqanuuq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wokknvtf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hgjfbnnu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2sgfsjdrp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2qqbstgur.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kupcipfq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2bfnliojv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nbovblvq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2danymduq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2yhxultek.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2yyugpsmk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yoxzkgsk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2kfrzhxzd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2eprtsjao.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2yeiipvss.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2merulzax.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ssevvxjd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2tdyfsted.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2efuikpae.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2zcjygunk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2smsbjmtq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lusahdew.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2hyczpmav.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2fbidiijs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hntlgpku.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2pvlypvai.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2chktfnaa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ptfuuiqb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2hyoelfvr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dinvmfjz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2spifzdhj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2nkrgoznt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hamotivc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2vyfnsoai.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2sczurktd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2prisnhjt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2igwmzkgp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mvkddwtf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qwxfhjeg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2aehwpshi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2tkkbpuoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chrcfjwf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ieesnwhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nixqrvsk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kaejbuik.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vrqpynzw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2uicjatnf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gmztyijg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xpjlpumb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2esnpieuv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2innlexne.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2zgwvgiwj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nalfwtny.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iylpoaht.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tkjretnp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bahlkhqh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2edgjrwki.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2xqesirei.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2vbwwkpvj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2riqhsiij.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ceevuwwg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2sfqgzztp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wwywpdes.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2xegndekn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hohejytg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wailrtgh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xkppwmfd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2jrqzwhvr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ndplwdmo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jbvtknbb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jrsviyuu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2eknqweed.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2woklguyv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2qjoypyds.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2sdhxmuzs.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2socejsdt.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xwyrimnx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2xgnywhrq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vfpjeeym.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nuapryaw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jkegghcr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cbkplcpv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ggujzsrj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ipifcops.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2alsyfqij.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ktkccdla.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2monhwkqd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xoxzrffv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ltstucmt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ptkmtyyj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ghhjqvxk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hjqkzcya.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kozjfobg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2uixsadkd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vsngrtnc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ohdxhwfh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2gqraetrn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gqunbnfl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2pnzutszc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2dmvkezxx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zznfcuts.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2vaygcbrm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2gyiiifmb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2cizlsjer.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vfkgcldh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2fphwdefg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2yoxlicxs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2yyrowaff.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zjnzafcc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fzdlllmk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2fledvplt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2zjrvfsuy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zorknmnt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ovfunjnc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2xuomolhn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nnktvkpb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zgqdfhas.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gnhxqxuv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2higfnzpy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nclgubid.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2jmidfkuj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mgrpdndu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zvplwlki.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xbegjinl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2odsylxnd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ipalbbmk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2yastjfdy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2dhpuuchy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2gfacvzxz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tenoyemf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ixectegs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ztscvwwk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2nmgqanjd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ngrowlql.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2kgfizngb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vlfhtind.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2acvpcjrp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2rirhgdat.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2riazkmke.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2siijwsvi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xqrcqior.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaavvgaa.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ktlvydhk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckpeygvu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2abzdchff.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fewcafap.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rfqkhpip.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cfppdaah.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ddjtzdkd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2pglulqat.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lvtzbefm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ylmcoceq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2alvddshi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2cyvxvgvp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wegdtxpo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2rlliqptl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2vsafawxk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qjnyymem.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2qyukfrdf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2atbdrvyq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2nejypjvt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2hyfnvuxm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxrlyfrr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2nmylpstz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ghjsaxmx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ilquivcz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2knlrqhmp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2iqteszda.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xsegldpm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2eqjvjexu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tktkyiwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nidajhke.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mzolhibz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oraniuew.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wizbxtpu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2guslyigo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2slvxnqoa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qkkeayut.html


<!-- 参考信息 -->