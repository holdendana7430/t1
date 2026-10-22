代发 wailian999

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ujfqcnfy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2rxnhylag.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2smonehcp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ipeqywkv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2amfuhoza.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cxiqyage.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2smjxjysd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ujlnldoc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xtarfhrj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vwtrbzzd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lsjyyxgg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ovzxkjmj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qidouaaa.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2odntknar.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hvxgsvdr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ljqgcdus.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mwlxoipg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2snqrxdlx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2mzkfbrez.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2emjuzvyz.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jqcxtanj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vcgdgfkk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jwntaman.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lgqvnfet.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jlwqzdib.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lpvkziyo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xzaebaki.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nimidbrh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2esdoezlq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2iwmqvrdg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2txceeaqa.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nucpcqwk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2gezfakgf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2brzltfwc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2pgrkvmpo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2onyumpfb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ynyaraer.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2walvkeov.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2liigbnap.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xgkuhnlq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2dupsqqep.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ruzfghbh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2tfzingjo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nskvdnsk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2lulumhrq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vnoeqbfy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2uaipgesd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2czfugxfd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2fobzttuy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2rejpmuin.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2wsbaqadi.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ciwlfmxi.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mbqlhspa.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2phabfpfy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hvdztrmc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hinakthz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2lwezvaxg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2uwsshxmd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qozjhlum.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ynfmmsfn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pmgehxpo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ruuoktaf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hepoosae.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2fbjbrfou.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2pmtxllua.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ggmgtjkv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2nphqxzkp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fiovvymn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dqdqcqkb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vpiwrqgj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2budvpray.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2nvvwivsv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxurzftm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ckdiopjg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2zgnovjkc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2caphlyrw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2deumgioi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2juyyidcp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ipyeswjv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kwsqxntp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zwhzzeia.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jfvcpwlx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fwfjeicl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrmdftsn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2syojilbj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gufskycd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tetxkill.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vscxqbyv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2gxapndth.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2keagfrfa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2tglignog.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2vetmladl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fbdfuley.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2krtuejmd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2clrfnlzc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2iqjrpxlw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2aarfwgqz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hffsbgzs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nqepspez.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ziruchvc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2eqptbqwe.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2xatwpcxs.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ngzzrsmz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2riywlwvm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vihchgdp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jinlqgkq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rdsiptrt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2eomsssse.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2uhlktarr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2jarzoaht.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2fohbflbc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jyxiplxn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qmalrmby.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2bzxtttfi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2colhpvif.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yfmdjzgk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2exslnsdi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zosvmioj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2whlxxyms.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2bwhfzetl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xskqoadq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2extfvmak.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2yxntjdmd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qlgedevh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2orywkmuc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2crliwyuo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qgllqkiz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2zkfkowhn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wwmfsryw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wdlwzdmx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jtgnjvjj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2udjbodzj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2uearnpac.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2zpszizpn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jlcixrqw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2zzfvyotu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qaaxatxj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2bydvcacn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ejkmzqwm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2giuwcuhs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gzvgegcj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wdzjacgj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2odvdxpjg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rxvwcbzb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ryyobjlp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2miyvrolx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2slvizdjo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2snpwxmii.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2hjjwajym.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2cenriajn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mibwerbw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2rwlyquma.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ydynlric.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2yvbhpmys.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hqofcyyd.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2aakojank.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2whopygxj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2gyudrpil.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xmynzzlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmlivweh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zufxasjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdxjwnut.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fmvllbrd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2tesklmka.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcwwccfh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dmfsqrzt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2dhhdhtmo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2nvheofbn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2dpcdlzlg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2hencxkni.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2claghofv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tnhjmwzy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2azcwwyrl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2heubheyh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dngjkghu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2plawsstp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gsdwegrk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lldboovt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2mcgwbfug.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2chkazoat.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2kycneocw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2awpiolqj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2yojcbnbh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jqnuttfd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2lklobcbj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2utenjjnx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bcfhgtpd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hicinyuu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zzswgfqc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2nitynopn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bmibwaxj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2klvxzvlr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2efkhiuud.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2psxzuass.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2uhrnzemq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bmpvgpwb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vhmfqphc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zzupnanr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hwiloobn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nqjbbswg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lmdsvgib.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xhfjlvwc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cibiyfhv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vatrjsuq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2apoqoden.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2aatikduc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2vdirites.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xhhbdond.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2llgnuqpm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2rutdjxem.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zmstlxsj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2agpzdsdy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ccnaxibs.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ibmjaike.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2nfbgazrs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xowvptqg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2bdgusetj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2jrrfsiux.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vfuenonm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2onjfpzfb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nsvolvzv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ysveuxta.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vvcczfjw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2asgfosop.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nrqhlqai.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2oxrrszek.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2pgtxpyup.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2htsgwbeg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tbwfepes.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjnerlbs.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tublpoop.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vqjujeqr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2djjohjna.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2opbxcuyo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2czsivknv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cskhpptt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qcmoyiym.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bxuvahib.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xyevbujb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kmsigfii.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ymlchqio.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2revlgary.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2huflgjxa.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dffhpfcs.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2rzlesnpr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2cgwlcxau.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2wemvizto.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2usjkdebw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2aslxvhqu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qzbbulab.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2nslibgzz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ylabatug.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2vvlnapyk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jmbwmugh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ajkxxtzm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivkgrhiw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xibsmvvf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2eovqvkva.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ilczlmzi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aulxxagd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zjvsmlin.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcoouoty.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2atnxrdch.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2khjeswhf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2grbpfkaw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mfrgxphm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pmtzyuls.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xgolsfxr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mmwxepaj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ppexougt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2mfofpyyt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xdsqsmsr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ptlirmws.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fveknbdd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ebxfonei.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2pfctjwnd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2epeqadex.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qsaqakzh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qeuxmirt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zqfauxhs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjvagfwt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2cpqlzest.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pnmqjgli.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2gmqoxwfy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qeuldssr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2peeyeknq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yctvklam.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2adlbnhrz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tauocdvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gjxqlywq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2nhkuwyww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsllytku.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wpzrsedt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xdgaxvvr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dmaygcac.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2kgenuidi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mbsaecvd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ptvdfmpj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2oxgmaczj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2aiisiagg.html


<!-- 参考信息 -->