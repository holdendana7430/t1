代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3cvlvzanc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3cxgeiexs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sgvtpefr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vtxejmzo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ceycpjyz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zrnsfcnk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hcurrxat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rlctsnqv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3bmkmcjqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlmywgrc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3nmztfrxm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3bpxmkxra.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3cqjtmttg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3plaouqvl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3stmumbbs.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ijxpehgd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3cyfrvypx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3higilbnv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3lnsaddzm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3deobvxen.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ykvzxdsq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lczbykbc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqclkgng.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnvwjasi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xlitmitn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wwadgmjb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rytndxvr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uvibfcae.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oepdidhv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3reyzyatq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dfomlzca.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3bzvamoxn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3bylhhoeg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3njvshzml.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3lmortwke.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ibbylaez.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ffdeutjn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ngxprjmr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zcxoqbjj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qnerstzo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mekprhky.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3vggsibaf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dhmiarwn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dsonjpml.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3utttyuqp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ohiugxyj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pxfgodsj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3wjowykbc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bgmhishx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ojizbbxl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ksrxlnrt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3egkiepge.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wgudduko.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3eyoqzsnj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3apeolyei.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hzldafdu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3inagprjy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ofuhshvn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3myzjvnbw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pgmokpyt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3udviideo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xgwdhdxu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3iooperye.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3uxftdqig.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hgnsuavn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rvwfxklo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3cuyjkxto.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tyggnjit.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ojeuacmc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3pdqfxwzb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3sbzeqeso.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kqldbyqx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3kbkberrp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zhyapaqf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3srqzfaom.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3cuthwtfo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrtgugkh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ulpqriow.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fifjvpgi.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3kewqlgci.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3naeetvoc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vzyzvoem.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ylgbmspm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3jugbfogb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3kkayqqfl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3mpkfvqlh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ucdcajmq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ogffzsgv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vwzbhqrr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3nqoodixm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wsdmteny.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ryuhqmzb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gvyewczb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ulosfysc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3onfatlrd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3djfxxtsw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ueipbygv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3gbaqxrgv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uigmwcpa.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3aueihxid.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3aopwiyvk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gqlirvbk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vcxvgjnd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3udcunlgy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3xdcgjcma.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3amqjjgph.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zumyqwxk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3dtvobnlu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kcejcoth.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wzmqopdv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ckoqpyhi.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ptlyejtt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3nqxcofoe.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3uxkaebqg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3muuvplhk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3epdebtep.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3kpppbdpt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3asndioxc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bkntmuga.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3lhfdalqq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3lamkmsza.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kkniemzy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3uvvlefzk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3kiqubeup.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dqygbiun.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3pwmqeiqc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3mimjncwq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3heoeenfv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xjskpbvr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3khpqucws.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3imzidgkq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hlwroict.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vnqsbvii.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mymdrwxo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xpfsilxq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3uulhmlop.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zxiucdlj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wpnjzpja.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ergzvmeb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3lfscpkvu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3doxojrlu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3fvjogewf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3xbxxseqt.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3msxpcewp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3dqtquxfs.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mbsvskxv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3fgwdvmpc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3tsoelene.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3bpodtegu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3knbfewjj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ureceeww.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3glxumbiy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ykowujyw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3wpcduetv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3uvdseibe.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3aacybhjz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3upucevra.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3pshhxqop.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3sixxmlrt.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3yspxrpsh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3cmhcyrfx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3uwvxhlpf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ldxinpag.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3fgfrehfh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dztjojwy.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3fhxwaqzy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3opajndvi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3madjdiuq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3yyumqbht.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3tfufaujo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3axevdzte.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3omcqqhgw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3tututubx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3gzqaijyk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dzazdipe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xeqjzram.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3cgxvcejt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkveefbp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vgqxqfdn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fhupmwbc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncoyexun.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3peelgfod.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3dmibweis.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3sozbxdrv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3sdbittvz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vglhsozq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rzfiheir.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qkhwmsax.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cssoklbd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3reovjxlf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3abogefqb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qeoyykvv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3mxybnkai.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3vbxjiczc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3dyxgflwn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3arodxwok.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wojixcsj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3zmaiztwu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rlortrtn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zxlpusft.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3pmnegxnm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3cvowshub.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xxxlafcj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3erykueae.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3waragnju.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3jktsyuau.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hjiefcxc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3myyagygj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3pcgqjopz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3eyqjwtdl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3emxxgoxy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3erxyxont.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zkkmmcet.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jynfvyfu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3qrfiwjdj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qbdljtoj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zpqerfqb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gljtpflw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kznpxamt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3dgeucwjw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3givkozft.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ahnkkdpg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3nlrnvvxw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fbdmplft.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jafnbfre.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hvhwlnfd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zjkdcrkj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ymsnbjxs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3onojjtrg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3wyztsrhv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nsgpegwm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3rxbmcfeh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3bewblkbv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ddfofmqv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hzxujngi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ohlbwvaj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dtjuzrsp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3rzbvveco.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ozdlupfj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3lhumklew.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3yscotcks.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wwrthhbe.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3plqxswjd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eurxgpbx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3shlrwpsd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqgsftyy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mfddhbdq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3gwyqzraj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3acsmtrrv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3sosmmdlc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3yyhfgcxo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3drlmuvre.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3bjeeheie.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uzgmdqih.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3phgijodd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ovywtekq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ecpoytws.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3asassxni.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ejbavqws.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uekszbjf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3rtpkztop.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wkqsbsel.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3kgyqjnqs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3legbpeqj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vyvcuojn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3npbycrrq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ztodkrrs.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3usgobhaz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3evctency.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rhpcfgmm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3omlatjkm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftnvgcac.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xddkjapk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ccaqlbjc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vrypvhyp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3fpkwxezi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tczvabqv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhhworgw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dbervgmz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3wejlvmxd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3nvxtxtcb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvpvirbd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rkmttlvt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xfpfcdij.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hfjutywc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3sbmqcdzu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rstpltqt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3dkfabqix.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3pxvqrael.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3klcfyfsf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3rdyxeidl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3fautzzpw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tiiwzmuq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3xnuvwdhb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lmjesnxh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3deupmzle.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zacdjvlf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bnrrryyu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yokcagyh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jsivtkgn.html


<!-- 参考信息 -->