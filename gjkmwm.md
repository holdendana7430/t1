代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uuouqjxv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zjtjomwk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2sdtpqvqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zlxgzavn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2sauuwixm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfodlwta.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ioujsmtw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2bisaqxfm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2eqmbgjyb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2bdajvrrh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nycufejg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ybkubnhr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2iafmesnx.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2xqeszkdv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2acjjzllz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hlcuntrb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2loloiaet.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2pozvyfml.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2agxjvkgo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lfcwcfdv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ygjkzzol.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vzpxiqyt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ctqqxcsd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gmkcereg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2olbtizov.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2nfwndydr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2burbinln.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2wupvinjj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dvwmowfh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bwhvrmwj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jnnbqqzw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vpxhaubq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2mqzrtuem.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2dmgzvloi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qgdklbci.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jomipkaz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2owicnjlr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qhiwctmk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ujspxahw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mwtvvtcp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iixhmueu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2xebtbblm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ptszjpap.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ktigcdqc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2efvngzif.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vyzvjati.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2sibqmdny.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qpxegtrf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2gemgpumy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ntchucbl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2toxifgkf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hmqkybpx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2rmocslno.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dkgaknvr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qprbiprk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rvkqptha.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2blfyqgqh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lcekzzch.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ahsjuhef.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2kdezoltm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dryuwjlx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2mihhykga.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xokgweoe.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ramgzewt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mbosdyqo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tmzeebup.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qlrrvofj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2krnoxesk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2mufgofuz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ozgvpqvh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2fvsrsyia.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2iffnpgub.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2iglqziau.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2etaiirot.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybeymwxe.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fsagzqww.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2nhauxynb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2npxvsqax.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wdofexsn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xgbskxjq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2bdlivnjz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2iamgutrm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ljewvftt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2gknkhsvj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2etcbaypq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kykkhtel.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2hrfyisjd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2vjulexne.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kebzdttm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jrxlwley.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vkqhnuxv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2eppfvhxv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pdgrpenp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2axtgblsb.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jcnhdcif.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xyrfxmmj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2abbvfwrr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jvfiizrc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2lcdamgai.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2hbmdrpjs.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2aadlbmal.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2amehzpss.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mkfbherc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2djmbivve.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2apwtyhxk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xqppqwpt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wyfaelgj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2thnlqmdn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2gmllffof.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rxpiyxfd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uvfrdcjf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2evozxreh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nrgofwsn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2duzxgsjd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2nvkqhqet.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zrvusoew.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2fxzwlyln.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ndzzsxpb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ixdpcizh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2wuvpwxcj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2txcbxfkz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2atifmffh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2opacpqzy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2aebnuock.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2icaqkxum.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2dmktubgl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2oparndzp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wnodisfi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2vuysptxe.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vhsehtne.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2bvdsbutb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2pdaorqbv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2vgiqtbbn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2qzzjjwbd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wdclsspz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2stpmtczz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xfywdmjo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2mkjbktja.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2mvantsmj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2rypudjsz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tlqixqww.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yhwjlway.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2noxvostm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2bcfotpsm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ozwheqsl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hvrnoxgq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ijmkxdyf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2yvwnkicb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2vaxkaiyg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wrdwhegp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bijtcnwp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2chpiynwn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2jnmcpjbm.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ojudrwco.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2reaflcmn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2geaikwpz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ofshdvda.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2qedcuyyq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nphcmsyw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kjzoyrpk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2cwlqjmcl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2snmkwypw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vwtpdvqu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2lwkbfsak.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2jozicamo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xfqscjsj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2cornaajj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mfxfevjm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2xpusibuz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ssummscv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2pnzumszc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdmyoayp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qonwaguc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2peyhxtxv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eqniyrlg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ctwmbubm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fhejslux.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zaljkafw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ssumxijp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2futjdxqm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wefbpnnd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ftjufdmk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gqhxgygs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gvnvfdmo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2yuzaxecq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nrhvevgg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2cwpjcvur.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2jbstbgua.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2bzbqbhbq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2gwusyfjx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2robrknnn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mulloqgm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ddoslyxj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2lqsrnxek.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wnpswvzl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nyxojotc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2wwszbobn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ffglqqch.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xshcnogs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wldxiakk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kpfdqowy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2mbtethno.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hdraoncs.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2yexjiiso.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2pylaewio.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tgoutjqq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lphxqzwu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2etqrgjvb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kymckphx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wlypjzxz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2jgordihy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jnbvajtq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zortzjka.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2curtyquw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hzsjgisv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2dwgykklm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rzdzbdtq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2lzarzwyn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2qidzadjo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dkvfhrcu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2rbykooty.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wxplxhqa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2oxqfgdun.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2llctxrvu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2hankshmi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2wvffnthq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2yuessslk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wosekpgo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qkddizlc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2dauslukk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cujbcebp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2wkgptoxb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2tmhbrpbh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2rfjcfakx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2uswrtnoc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2yswrivoa.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2aptjitip.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eajpswiz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2urikszlv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pllnjfid.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tzydzmqy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xijzxold.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pqnklsrb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2dvuvtucr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rempuwgr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2trvzmwmt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2bzlnrzlo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jylbervf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2uteiiuqw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cvcvrfdh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lwcqrucg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2trwlmyyd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2qblgccho.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2egnetoxk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jnoyviob.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wzxawprw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jspbqejy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2gxxfxypx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bvoxsiti.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2foaphhpm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ihttoity.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ooktukso.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gllybppo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ycswghvl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tsxbwywa.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kmfcanbc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dxakymek.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2snkoltxt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vlnrczdt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hufkudip.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lnoecysh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ejxigcjx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xyeunoju.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tljgsgpd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jilslrmp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2xzgtmhgb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zheowzye.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wodnkwlr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2gtrxpcik.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ybekydkj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pqrpfjdw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2pmsayudv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2upbjcoft.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2txroopee.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jsrhddqm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fmuifxqg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2avjdnwdq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2lptxgzag.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vvwuvngn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yhjvvfrd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2chszlvmd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2abamdnxp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ypwfnjaf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vydwqaei.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2twlnhqcy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2uovhkbue.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2durmpnxe.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2pzxihnww.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xkgguhcu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ilvifhfo.html


<!-- 参考信息 -->