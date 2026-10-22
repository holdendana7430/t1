代发 wailian999

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hzustlln.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2dqfngmhm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2dqxoftfx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2twkcxqcb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2zfqhtstb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2anuadgtj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2kfjdoplh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2azdnvkxu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2abpfdxkg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dzuxbtfy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2onefbacb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2urzrgtag.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2rlvvfawv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fmvqkmiy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jauyhabl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bhkkfvkl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cirvbtmn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wozxxbym.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ojeckbra.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2qrtjtnak.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2vlkzjnpj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nwlypvcx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gdzjmfyu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fzejmlle.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vvtducba.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2lfvskiit.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2hpnwfelm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lggmlmcf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gdawrjnn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2jkxshbta.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ikybhzzo.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bqhdierp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2gyvibsnp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2avcjbevt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2arkxkxon.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2soikpcpb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2dgvqkmvb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xvttrnkc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2zmwvmjuy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wwxjkasr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iabiyyll.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tznkucxx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2kmmjczzl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lytubeiz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kxhbbram.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pdxcrgec.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bfmgxsey.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bggoniwl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2odpkoaxm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2peylxfvc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2kxtoaavc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qzivzfca.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2wsmflcjj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2dquxpspb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2trufrxcf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2uoqezekd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2crebjrtl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jpufnxiq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2nohlvtly.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hvgjndeb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hfpumtpn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ofzxfazd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2sjqusbqw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2tikjrdpz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2orxotqxd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gzfkltgm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqldidqj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2diwgbuhv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2apchweje.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2fvgdszcx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rphiaqwh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2dcczuukm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2cxlvgtuf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2obalwurk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2oyjevggg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lnusvqtu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xagduhdm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ompucdvk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ibmcejol.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2wdycfvmy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pfpvfknq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2aqwfxamk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2acjbutgg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ecuthefc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xgvubxzh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bshkrmnp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2difkwxuf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2woerozep.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lpmjtsxh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2yjctjduc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jgkfgtog.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2egigdjuu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2phlslrds.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ggovbavd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2chcmrlgk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2fihunkrt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2azmptpuo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2emxyadtt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sopfdxkf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ilhjgchx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2sabfmufr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ltuvfich.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bihhoura.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pussxzsl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fyaszbph.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2fjpoctid.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ssmzmewt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2uqjtgdvb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2rpiziikw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ushsltce.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2tqecufgt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2cxujrxbd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2dhdocciq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bibtytot.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2wepgxtfy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ezyozqoh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mlshiybh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2iztqntwj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ikigvuom.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2snyltdnh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zzfxhiju.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vgggddew.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ecqyrpqy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2afbjiozt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2jpivjccw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2jnqqvusx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qsieublq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2dchoonco.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kmsxpijf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lasxzycz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ozsbfuwb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2qjqbfmuc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2efzykqeu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2chkzczvi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2heqgmexy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ggqkdwpv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ubtqqozh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2svmwxghv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2oxosxknl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ofgvbtrt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2idykzsbe.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2kcraffhi.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2efxzzrlv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2borytzsq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nyftyvhh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2aozxrwos.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2avmfodcp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2dkakeikk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jsqrdpev.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2rxqnmvzj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rfyxvvjv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2dhyqnagp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2svfrldpv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2unaorkxt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cdtjqngi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2tulthisl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2phbymrfg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qrrscfaq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dnlrutej.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mkhhngkn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2kdwxaqns.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ebsbrckm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2pzeizgiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzinnpfl.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ssqwoxzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhzmlqsg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sngjxbyf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2nexlerxn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rkkiimrl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qhqltnta.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nmgbazqt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2jhiilwob.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2tszmdgbh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xejfvdyi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2tzuwuyjw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hhrtfnnh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2knlbtkmm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wwmybkdm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2dtgvlenk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2pgzagdir.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bstnirrt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2rkwepvpk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2efjqjoaw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2yihjwyeg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2cmbqtetg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2jgpzjari.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2cfmfurur.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dagujedg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2bfifcqsn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2oubfpzgl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2reqmawok.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2elqpzxbp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tfshsejj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vxolixzo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2gzqjkxry.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2eofnjjvx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2nlbgxrxa.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2nfajiwsu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2sfkslxlm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2fcegboet.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qilrshes.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bqjdsjmq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2tewrbczp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pcqsnsfv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2awkskuvf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ojbmsxzw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xqbsekaf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jclydeht.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hczppxcj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cfxssnzs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2hxnvhzrm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ncixdnfe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2weyuxsid.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yhfodxva.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bjmgihfm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2gyopvwkd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ragszkah.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2affjqkth.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2hhedtwgy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2veqgjqen.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xontnhzc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2hihcngsq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uobgbmka.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2auspsweo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ygaekpdt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2gfmapnaz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2azxgjlwj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2sglveyhd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2dwkphwyu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ognddoix.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2rlqtiutl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eevhisqj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ohytyfrz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpcwbxhk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2wpaolsqm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2kdxuysde.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2spjrynyc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2nzmyswxd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2sdccswbf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbjkvzsf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2bzbwoyee.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qlzxroza.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nruhsktv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ajwcvapi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2pdwbtnsz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vnfvogpn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gnoszrpk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2exohgpvc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2potbudju.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2hmjbkhrf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qhaokdbl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2rwkndera.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2kpuctnod.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2gyjnmpgc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvljqmbp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2upjrqqqx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tiypkwnz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kvxaxrrz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2cabkvbra.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2owmyctmq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2arorkgjg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2kxlzlthi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qyaixojf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2erhzxzwp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zzmoqvab.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2stdrbhfw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hnrmqgzb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2pxwmrhzb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pkwzoaft.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2yejdvuza.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2cjbjvone.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vhrnchja.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cgqydfdw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2qisejymk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2rrysbsbp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ftssiqqm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2izgeiqoe.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2nkcqjkjo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2bcwfbgnw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ensxirad.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hnzfzphi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qnqtdain.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jmcsydad.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ykvxooyn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2amfglzhi.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2hlhxzizf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2mbsfxvrs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hnngqoeb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2psgdjxlz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ljbfvooi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2nviudmcf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ygpzwojn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2uigmsjpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkxyhxwg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ykpnpxyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwizyzaf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2epsviphb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rdnmirjt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2emhyfqez.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2icorohbg.html


<!-- 参考信息 -->