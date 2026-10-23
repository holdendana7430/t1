代发 wailian999

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3fbgjknqa.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3usgonkfz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3htdgpxxs.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kylzkavj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3vjfbckcq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lzmhzoux.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bdecnsih.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xfkpupxb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rghosnbb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nfmhzjyu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ojgoyzqw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dkumkgnd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fzbavoda.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ukrohtim.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3keeuigwx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3hdbnlowx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nrmqbodw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3exanxemf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3juxwrjfn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vcczkshi.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hqwginyl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3wadjmbdh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xwosvofx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ymakfzzi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zzoceqfb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nsvefccs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3olvkzktt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rbrxgiom.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3rulkusiw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bumqjzhk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3facoooou.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ivhiygmc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3puixnjsz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3opdxskpm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ghvidyfr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nlpvubqt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ocwhxgaz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3hmviesxn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tawdhvor.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ekxwlhok.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3qyacswjf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3moafuwaz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3hbcbstuj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tmsxkrzb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ltgemzqh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3luangrnz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jrylfgmm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jvtaiiao.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3cpfhldov.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qpepqnmr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mfkalhaa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3epzosmtu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3dkyspnjv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3wefmchui.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3vyggdnkz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3smxynnjd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xswvkolk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xghlydlu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3qeozbjub.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tmxehrod.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbrlzxvd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3znphyguj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3imrmjvlq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3urttjxpj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3pfgutnni.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fohxiorq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nstmyfjz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3idvpppnf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3nrgcfgks.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3drtvgcib.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jciaiiry.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fgzngcky.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3uaylzdzt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3lxipkgtb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3uhaqwlpu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3gpmzedoh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kzeeqogi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mffvjscg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3fhujkqlh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nikkqihi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dvqdgffa.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hkycxwlx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wmoymfuh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wauojyto.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hsmmfqgm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3dheqkvzt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qifhrktt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3hjwujvut.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ytjyjxfw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3tmudmipv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3oszmfegp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3iphaopyg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jadsdwlg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3kjpuvfet.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jemvhlwp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3dzsbkstr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3rlfashbc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3cnwrujrl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pzuvbmzr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3tdvyobbq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gpcrlvnp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ruksfura.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3axfvkqsw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3trqgikit.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ekikcsqr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qzpumtfd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oydyyoba.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3idrhwmes.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3oyhwlsxo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3saroaqli.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3oqzrnwsc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3mgduyrwu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3dtrvaeld.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3bbxwhatd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xbqoadwe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3doyfcynx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3gdsdhapq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3edyiszqq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3unyvcvty.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3fxipcnts.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lqhyhclk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3gciswjot.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ozjbhggq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ccsjhrcn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pojhhqmi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3hqonmbtm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zsocijom.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3kalcvwnh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3zmmpeoke.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3nzllpuki.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tjfewptv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3dpcrftml.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fjbjaozk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3xobegxfe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3umtvjjpa.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3lcupfrqv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3fejqzdqx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3mkxbwfyh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3udkveatd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tcpozqra.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hrhddqbo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3okelhleb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kjjminvo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fvduhwmf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3tczwstxr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ydolherf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3pjvqejgq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3betvmgdn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3hgwsnbid.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pbjzhxgn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mzzxajkt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bctpomtj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3sgmhahdd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vgmksaaj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3fvtxdifr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3amxfohon.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3hrcflhkb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3obxmcykx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pyxmruku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbkizsfs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qcgqwmem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3asnnlofk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3baqigcsu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3sgttymki.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3behgcrhz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vuclfbpc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3eenhrbad.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3aqdxwvjx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lsugkevt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ifffkbhc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bscxraao.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fvucvyvr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3weynbcth.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3iugnxszs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lrjgwtkv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3lswhhiot.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gphcoajd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3xqdsdlnp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3hwndndyb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dxigudcq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ybpqpvwc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3oyhagcng.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3fhjhldsg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gggfhtnq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3aidkuvup.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zkhtgizd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wyapxiyt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wpuqucfe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dsxhwxod.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3mxoxmuqj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3spiomawy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3frdnarfi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3raosjjbj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3iniynoqf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fivwywox.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3gnsxmzgv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3pnbsqosp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3csxadhpm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3vberejdt.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wnbhjlfa.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3qdzucowe.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3sacomjeh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wopmkhsy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ihuukxqv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jakybwvw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3svceaznt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3iijyknmr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gbnkrqdn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3xvluzwfn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zmbjqscu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3fmjfwqpa.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3jcimaidy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zenggugf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3eghlaxbz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3efvrmzwl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qznncvcc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rnytrvzo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3mulwsvco.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ltiubuvz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3afcnitoz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3kvalbglh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3lquwqlrx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3azqpmkbr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3jkxjrimi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yvwugjai.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mkokwxzz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dzeiqgtw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rgfgnbfb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3zucirtgs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfyuifee.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rcwrzymf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3exjsyely.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vyzovsnu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3erdnsfjo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3gxjbjwdm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rbveioey.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ylybckfy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3axqdfeav.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jmguykwv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3floxllsg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3medzoqwh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3esbvbgxq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vyacrsjw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xpzfltxd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qsajrqzi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pezstdvb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3pegulkou.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3gsfvzlax.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gupdpekr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wiixbbfp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jaipyllq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3gneeqfhn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mftjjkup.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fyklhvbi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3sntboqxa.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3aiivoivs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3unglwbbw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ygvpxlxu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3kwdccmhu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3slnxakuz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pwwyzwpz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dljjixlr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lrjmpynd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3otcybmoe.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3llvrymrn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkfwmrbb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3kszgbwta.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gnohgrxl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rvievoxo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ipmckblt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kodldibg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ctevhsvi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3eerwxued.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hjrznxyw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3amirhiiw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3hgtzzmav.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ylesiccl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3oyefjazg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wkjldyib.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kayvarpf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlogijhy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3irtectzx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3qgltyrai.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ubqjcfqi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3uetoltkx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3javeelcf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3xgrznqyh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3nvzzlydy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nldzxpze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eccgiqoy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rezgadrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opxabdrv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3njjtduxe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zcvhtipo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fykxuaey.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3jbzwolid.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nlbgebla.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zsudytou.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rhpxmzks.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hgkodocz.html


<!-- 参考信息 -->