代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ajgccakt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3liglzizd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ygpopdhx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3wylmoqlf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hwcbuytb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3fzdlthyg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3yoausxza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgdnsvzy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3yejgzeuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3naaykoqb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3qhbylnhm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3smvmuffg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3sxxtsrfm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3pndbmnxf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3varyeohh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3pllfjbhg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3mfrbktzw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3psniwada.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3sqabbspf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wkwyfhcc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ckrrpjwy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3baivisia.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dbnporob.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ckspjcmo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ciqxqqfq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zgqtxrzf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3lhdzoyxt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hmemnzxw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3oftvafcv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hxrpjwpx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ukmktnmt.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3gyaltwpc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vblwxcrh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3orrrovyp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3tffdyhlk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kxlbgfsz.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zlknvngo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3pglxipnk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3yqvyowvp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3crkkskgs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ltcrjmju.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zttysgol.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fvqvyjyt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tcfqechi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mvrasiux.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3bxspsjah.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dwzzokkc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cxgcggaw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3aakteulg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3jwiqqype.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dxraezax.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3unpwmufv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ncotghed.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3hhxxaaab.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3tcakirro.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3igwxsitf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3lxxnhvzu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kqmcugyv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3tumchgzu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nacwnwzu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3axorelcv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3erroibub.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jprvxqzc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xllmujgs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bovbiots.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3dorhccsc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3kznqeojl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3nvbqoako.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pxpmbgqz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3sngzsvzk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3oqwwsaiw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmllfzaw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hykvzfxc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qvargjpt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3dhyzkmem.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ywvihibs.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwlrugil.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3uwrmfaur.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3axsdtqkt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3npcgtgyl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zmhpollw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3rgrkiupv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ycxhzudh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rybxhztz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ccrrmkvy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3kfzrassq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3nvuggawb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3stemqszd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3itexnrzb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vpovpcjb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3zmlefmow.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3yomvdvdq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qpsxxjtr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3qcooszcl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3qvxuchkd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3kwtxiqig.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3muakthqy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3mjidevvr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fqfuzdin.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3znochqwy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mayfqkxy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3efnwnxsf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rdphwwak.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3jbgrpxrl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3kfhufvvz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ehdauara.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ljoibgwz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3duvqpbem.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3evqodvsa.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ioiseuva.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yxjejmhs.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ostxqeft.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zscvoafx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zejalttp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wfuwdwid.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3crqjfbzw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ynhzecde.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ohtyntsw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bfayydaq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3tjjadatr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qxmfeuui.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ehsflsnj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3luopculq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zxiuytqd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ruuezjeo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jjfutxmi.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lewvoryu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3qpemxrlb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3txsfswvx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3wqwhpjzp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3sldtbpqd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ezvzbzrs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rskuvdia.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rxwxeemn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3arjzysxh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3rsdsydak.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ulxioyqt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3casrezrp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xjdjjjzr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xmhfhqrk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3mrdeireg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3uwazprjc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ysdwxjwx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3yhlwmazo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3rwkdupqb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3isacwecr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nujtcrlo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ntqhyzmr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3zivcezao.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rgvuixkg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3bxznuvja.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3oqgqwycg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3uvekdkaf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vefawibc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3vxfwuful.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zyrxgjyq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ptslwpyc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3jnyytdpc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3slbflvms.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3dugnfpiu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ovucjgah.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3cyodrhff.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jzdhfyvf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hswtizop.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3fvsatdmc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3engxwpkh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3putxjoda.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3itebadzv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3lwmsemzw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xotwbdgm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ahgpiqce.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3vvwhacwo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vadshyio.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zevlqjgc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3cvajsxyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjxthndm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3nkqhtcex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebwkrccg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cbujwefr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3wolwxlas.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3dybvfihn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3tkbcfioa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3dgyvbkyb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ylhcwpxo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ijvfwvpg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3aqphqdna.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qjslujpv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3eybuuwwi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3wzdnrmuq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3iilsggsi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3anhgarfi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3qcujswwz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3zicordsp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jovhyhmu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3rhzimvzu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3svzxnteh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dnxfsfpk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3fqquixlx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3loahefsj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gqzzcaho.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3aioevnml.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nwyhznpx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mzfvvxvu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3souapzkh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lvyrlmsc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3iaxdpuoq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3oignmucl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ebdqnkof.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3bedoumeg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hailiqok.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bpebauye.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3pmwgzduc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ufdzfhcr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pajuifep.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3yxjfnudj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mwnirllc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3wwvpgnqv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3khvrofab.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pbbhyyqr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lmtdkrvc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3geofkguo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bgkjhqjg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3thxlzgvw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3odsumvpk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ikaxknpu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3xxkzbwne.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3senzhndl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3foatwbgd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ayhavqbq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3umowrrbz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xxfjdnen.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3yzyvkbyw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3erwbigek.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yyzipaqh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bpwwkqcb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3pebjsmjb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3yxvtkrvh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3apmcmjlk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qckkqelo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zlxmqeih.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vyzrobkz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hcfurvzo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3bcdvtgyw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qvedzvfb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3enxkideb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3srndxtax.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vqricfzc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3adnlrcpj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3zywmqzup.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3yklsocwh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3oxddfnac.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3jsfmyxlt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3uscnjakv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cpyyurna.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3plkykshk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ixvygewv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3epaxzeac.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3jtpskfuj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3qyldswbn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wptqcfzv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xyhgqfrn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hvefxeny.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3khtyqnzj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cwjfnrir.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yhpcjmsw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3wytndutr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3btrhbcyc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qwdwikmy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3nzuwahsh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dftjzgln.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3crmjacel.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqkcmhgq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3izjbcwlh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3pltngmla.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zfeatmkr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3bbewbmgu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dmqssdrj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3yauozsgr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uuxylkcn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ojcgcqwx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lcfyrdar.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3oamaruus.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nndetsmw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kxtbopet.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mxvtxulc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3xxukgjkl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bpjqfjlv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3qgsnjppc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3afyeveir.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3qnuhegvo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3gilwajaa.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3nfzwcoiu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qnkstxjh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3tjaytdkf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3krxqoprv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vqvwiogj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3vgewjurf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3mwnrluei.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3itrgosrc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jpcjplbb.html


<!-- 参考信息 -->