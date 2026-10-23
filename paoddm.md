代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3srfpeffn.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rwbuzijh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3iowhbtfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgjcykil.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lxifhqrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buyfsjzt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3nhuqhhkc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3yulzskbk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ffqdzaiw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3cusmjdvx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vrrncwqx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3eoqwtuve.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dofmufpy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zbbbeock.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3pauigqjn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3zwqcgyhf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fzahstat.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mrceesbi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqkiasaf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ruyirepn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qaostvmb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3onpujxwl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3gzxouybc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uyvpwowe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wituumng.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3qyaomneh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rfivavxo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3djnyatmu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3afgxoyvw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3kgnoxkpc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tgzlutuo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wqwvcnpi.html

esac
来源：http://www.52xcode.cn/Article/details/gt3sshahxxd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3luupfotc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3bwmxmgdt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3demxxajx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nkwnincq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3mfncwbrz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pmvxbddl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gvldsbkw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3volwznyp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3gjlcqfka.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vrahdvnr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gfituiyo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qhnbedai.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3jstqslwa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3pmlsytra.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fhxspxmy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3clfpdtzg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3rufhgfbb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lghohbmr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nkwdmrcv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3islamxsu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xguyqxrl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3oppsrjhq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3uwczkavu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3dkanecon.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tqthlxkc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ighqbidy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3gneidtqd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3znsahgej.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3odtejcdx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3dizsqkxs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3tthplgej.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mnzkguix.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dbmfffry.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3cafyxlwa.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vhtabljn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3fowhlmpv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tydwgeiu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3coslruuz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3odcgxupc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgwtqkcl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3sgctexhd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpgzibqc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vuofypas.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3jveujaqt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3frfeauzw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dtlqneqh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3qvqcfgyh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zwuptjzk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3acavcifz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zhhkbspk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3yvbwfnny.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ffrasnpc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3vjqomxwl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3qqsbasiu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3dsfmhrav.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3prdqafvx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mjhiowgk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mgxqxaqt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3rmveyctr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wwvhltbx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3rltfohek.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ododlstm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3lqvmsisi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kgikecav.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3juwywsfo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jpnhfcrn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ppqnskth.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3mnetltvi.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bbftgmqk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ukietfag.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3yzkzkozt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kgcnmxhf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bxlbdatm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rkbsvvlz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3cwpfpsfr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rhnzxjba.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3eyanfviq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mqryfltk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3alegnzgs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3kpqkguzh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ytsrkplo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3hfvlffzr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3rzzkcnit.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3trgogtnh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3otrezfle.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3lmemnaqd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3bpyjiyal.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ucsdxuvy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3alfbqxie.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ecbhhjuu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3yoxlpwmz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3dzzbgcap.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3lvfwmtnq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3eaixprpx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nxxgrqqd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3iqtxyflq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wybmzfqq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3beniohch.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3flhkrgjj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ddijluty.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3suqjwtrx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3woiapjsu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3llaugraf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3sgahbxtn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3niwdzxvv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3okmuywmg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3domcoxtc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3cmfifxrc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rxlyfdxm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3jpgmsmgl.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3etpxycou.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kngjuoki.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tjyqouxw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3tfrnhels.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3pdrojiib.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3oqulhynk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ktucwopf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rlmxlbmy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3grslnque.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bclfzyvn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zemlcoaf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ulivocgd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3uhhvzgmt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3glwtbzzj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3dzyznloe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3cozlfvaf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3tixqymck.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ghrrgols.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wzbxpmgu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nchqyfpa.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3hlkdwygl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vknaowtf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3cmpejmgd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3kccauhid.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3akpdhfix.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3krnbfkfa.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3cakbadlv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ciepowsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cybvrewj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3dceygdfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dlapiyxy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eizsaeps.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qguiovpt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3qqdslapf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3tebbwhue.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3kcqiwnyj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3hnoqdmld.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3slbzpzhx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3oyrixwkq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3awmccaqc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pxspwpaq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whfwpjvx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tdxtwkbk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ocjjzmjz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3byjcgqeg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3bbtycmfa.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jnphhbyv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3evpqkpuq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3abvqknyd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ahnnpoah.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3kmemsvaw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qqldpldz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gtfovzwk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ikhdkapa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sslvzeys.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3iefizgag.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3tfytmygf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3szqqlpoe.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3afdhjwkm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vosgozkt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yofeeixo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3bvewgsil.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3awigsddc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3qswijmdk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3bzvzuzzo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vnqzhbbf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lvoistcq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3obitvmjz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kntpykdw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3cvrnkwga.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lkkctdiy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mepdgynq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ikjrgjbo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bceqfqjh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3kpcdpzek.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3anerkrio.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lynnbjcx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3axiqpyio.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kpsvcwnz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3awcfivpk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hbsizlnf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3afnurqcj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fjhmqutd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3yrhjlpes.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3taibjjub.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uxbwowez.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3iitlctzq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vwkayrzj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3yscwvwkn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tmdbelmt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3reqcwczv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3owtlatui.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3roqpcjky.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3dabanmvc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qclngmkm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3fjpyqdds.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rmpmzbgl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3yaoludbn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrnmtfgl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3tplkmyji.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3wbtizyha.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3cchjrlkp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wcymoubq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ovixupch.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ygnawgmm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3uzhykkcl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cjedyrtp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3sxhurzqc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sopofnpb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ywffbgrl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3nlrilcaq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dxevwxrr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zpozkinc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3banuzwhj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3hpvajsnb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ljmesshm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ybdfzodo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3glbmbnrl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hmtoavga.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qrgchqzs.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3snoofmxj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3nwqmkxcw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dkbqbekr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xnmxrfhc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3leiwulge.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3zcqeidao.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3hfknnhtt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fxynilbt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3psuhaxpm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ulrcxvig.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3uhnxaajl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxdwgmry.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qearhoqv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jtfyqcir.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3yvakbilk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3feepikqj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tgajpipb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tjkehgez.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3geyjviga.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kkwsvcxg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3fzdczvlg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejgnskkh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3kmqeejbo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3eudlohgp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3nkrhjxxc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hknnzzqx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ysibizhb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vjoawrkx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3rpucfhmc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfwdjgic.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3rndfokvj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gmtzmsff.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ygmunuuw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zkvospfb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3udarkzli.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3mvqrydbl.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3vgaavsgp.html


<!-- 参考信息 -->