代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nmiluntp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wpyfugmi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2njlbblat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwmlwfdy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2uoswjpeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhrqroev.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2xcgruujf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2utgkgekt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2nzrnxuay.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ygkgpndq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2coawmxte.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nayqfclq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2gxsxsrcd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2scwhjytt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2krtjyymz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gqybolxc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2sdhoicqc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2glqfspzj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhuwieni.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dlktcjwn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2qvrfylvm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2bauvfzck.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ewvpawdf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zzubgnru.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dtixdckt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fdiawizt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2deaubymu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2xlrszmiq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ckkwdqvs.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2cbchbzqq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2syljcexc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ywvxkotf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2dbrwvtbc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrfgzbnf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2memknicq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vbguqmdn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2olmvdvrd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2vdlrvoug.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2puhlnvpu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kxtrgzfa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xokxhchj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cnvvaifh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dfrrbknv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2diuvawwl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ayksqnal.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xbmziwaw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2wgxguche.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2npwrlblu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hyyttzys.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ehxdpfyz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pjwbldav.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ptirhpzt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kznxzdso.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yovpgvhl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2givggtgo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jwvrndzv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tzynacqd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2menmtrwy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jphownfu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xfoiscid.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2iucuuovl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2caxojwmp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2nngymyuf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2rpybjpiq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ztqdbinx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tngjpatj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2yysenjwh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bxmraots.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ywmtgsvy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ndqjgcux.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2cfcdurpg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kgnibsob.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ipwzpmnm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zmchotyg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2byxynxqq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zceqiegm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2lkvzvjcg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2hwjuxcbp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2uimiyneq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xwfjndnd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2yfvxvnwz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zivyptcz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2euxjbctq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2nnodnehk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xuajbfpw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2icceomxx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ufeckrzj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2fvrworzf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yjpujxoq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zpjrbhmz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2pxvdpwqd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pkltysvu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xvuzcpse.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bfnpmadm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kwysigka.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2yddqkjtj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cjuyujpv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qurdwgnq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pnhydwtv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2mqtaoiwq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2grvnqwcf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vjsohldr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2npsllnfa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2orffnziz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ukpeqgah.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2enrowdru.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qqrylrpp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nygnuzqp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2fbqvttdc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2bzcxqrpg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pcydkdyc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2oeuoxsdv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2nbdxjnjc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2hqpimhvl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2mrvjqmmh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2npmfyuas.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2iwugmqdl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jomdxtft.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2nflituok.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2babrxiaz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2pgcflmrt.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vuwnmqio.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2yyrmfxot.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2dfogdeng.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2bazotlzu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2edfaphba.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2cijudhch.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2efspbnon.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2otpmybty.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zcjekvki.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2fybbelns.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vpwwjdje.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ptzzfyuq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pbbwgsrn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2cuxvsmbc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2rcrekyux.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2eemxvprz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qquqcnkp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rbzvbcmw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2iqhldyvi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2suqctmnw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nfszixkz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2kaeirptn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ymyulqxl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2oicphvfh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kykzbjdt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2hbzkzmuy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2odjezfqu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2rsfvlovh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2cgzyssbb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2dcumfkge.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tsimdvow.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2vfhlgeuc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vlfqkmfi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2srgdbryz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hhkhmyyg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2sckmhnkn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ujzsuaym.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aadjdzsn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2aozntgft.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2arfgtpqb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2bxlqbexo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kqgtofbk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2avktxxgg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2rgvjbmdl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2schmekbc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rouzypoy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ryzxufnc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2udrtlbxy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2elkmtknf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2idgjsrvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acyreiuw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bvfovbjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvuuceee.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2owbksxjb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2dyrgxoyo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2klrkcdeo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hdeqkrph.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ghnvjiew.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2afufohip.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2uesjjvaj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2faoevnnn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2jzycfjvf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2htywcnry.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2swaromqr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ywpjhlwt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bobjabsp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2obbzxfkt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2sufbxgze.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2vljoycbi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2fpjfhexq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ebkytzpw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2cqpzgapy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2dkvtqqsa.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jbhtwtdw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iomjqrds.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ljoujirw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yxitqnzn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nklytzyh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpjlvvjm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wbqzahvl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2mtwzyvxv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2oepnlutx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uqjobgql.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2pwqkdfne.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2rhwpewbd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xiiaplgm.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2frtwjymw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2mozbyqwk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nslzqfge.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rydkjnay.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qjsgmrxi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2gbursdbl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pugpwyst.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hcgmfitb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2smyjmmyx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cjchgrso.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2yysfgnye.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2cpjowgam.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ualfbwhz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rggndeta.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2elvmzkgp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kpshxcbq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2mrlrgfwc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2owdahmzk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ncpzytpa.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2lpvdvhnw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2itnmkryf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2sqwkpcqv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2kydxlibh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sdtpuylu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2solwwwue.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bcsiqyzc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tubhbrrn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vvtcdkpa.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2glclkccb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2predogvl.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2udqdyjtx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wvczjcen.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2arpjhuzj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tmipyvas.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbwvjhge.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kyemmvuo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2immwwtmq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rlvbdzfc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ytzjunwl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2avhcqnku.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bozwvcbo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ulomutwl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2anykeqzv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2buieoqeq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2crwpvrbi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gyzyrxhu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vpzhfwvg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vqksfnnm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2othfggvu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2hywumxut.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2lrfyeaur.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2pwqmmhxo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dhisoilb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hdsmrvqt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2grpfpcbs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jmbsuhpq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ixpxibmg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2vggevkhz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wglddsbq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2wjfytcxp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkrvuehv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tnmuupja.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2legjtyla.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ajgozurd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2whrmhofb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2sjtaxlez.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjxmxvoi.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jjyknpzg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2blrzboey.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rkjrtlhq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tfrfyqgs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hfbxoqxu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2lbvjmrki.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ttjpmmvk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2knrnvikp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2jkwetwku.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ylchxzud.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fodviofy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2bmynncus.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dizhbpzj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2noqolioq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vlbupznj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2gqmnqphr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ojeayfnk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xpcvduqi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtzekdkb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hhkibmek.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ukehunkb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dqmouqmp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ixcbrbvt.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mvnvkunl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lkgysgxs.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2qxlrlrut.html


<!-- 参考信息 -->