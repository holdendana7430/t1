代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://hz.hysaishi.cn/gtardclcde.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yvedp.cn/gttqaqjdaj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.dashuyun.cn/gtkejsxeom.html

[Q89] 判断表是否存在
来源：http://hz.cdnleiting.top/gtpalaxaji.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nwbrower.top/gtoeunmetc.html

[Q90] 生成序号列
来源：http://hz.dianchejie.cn/gtesrdrnsz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnxiangtu.top/gtlhvwlbhm.html

================================================================================
来源：http://hz.shzxlz.cn/gtgqsftjvf.html

R. Bash 专题
来源：http://hz.cdnleiting.top/gtaftntwxa.html

================================================================================
来源：http://hz.dianchejie.cn/gtduywdyno.html

[R01] shebang 与严格模式
来源：http://hz.quarkkingdee.top/gtjjqymuqn.html

#!/usr/bin/env bash
来源：http://hz.yuanzhike.top/gtcllvlfxt.html

set -euo pipefail
来源：http://hz.gotoacloud.top/gtlzhstdqm.html

[R02] 变量赋值与使用
来源：http://hz.zdqjudy.top/gtetavogie.html

name="Tom"; echo "$name"
来源：http://hz.sufxvd.cn/gtpsyivxay.html

[R03] 只读变量
来源：http://hz.kuanghao11.cn/gtnkubgwvn.html

readonly PI=3.14
来源：http://hz.tanke756.top/gtrmtwsmsg.html

[R04] 位置参数
来源：http://hz.ydjk.org.cn/gtdaeuadgh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gzhubu.top/gtwsafuwmb.html

[R05] 参数默认值
来源：http://hz.shuidangran.top/gtndffpvju.html

name="${1:-default}"
来源：http://hz.yvedp.cn/gthbmwoaxi.html

[R06] 判断命令是否存在
来源：http://hz.aibaodan.cn/gtreksghlg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangdashe.top/gtzxqhliad.html

[R07] if 判断文件
来源：http://hz.jiagoushi.top/gthrxqgycd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gogol.net.cn/gtibgjupne.html

[R08] 数值比较
来源：http://hz.ywan-chungtsiang.top/gtcujfwilz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sxryk.cn/gtwlhrdvaz.html

[R09] 字符串比较
来源：http://hz.jinyuanbaomall.cn/gtxnbqxavk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xinyue.icu/gtkmddgwum.html

[R10] 正则匹配
来源：http://hz.chenjidiqi.icu/gtebycmqph.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cdnleiting.top/gtfxbyoqwo.html

[R11] case 多分支
来源：http://hz.shangyingyoupin.top/gtkcwwpmwe.html

case "$1" in
来源：http://hz.yonumen.top/gtbrusildo.html

start) echo "启动" ;;
来源：http://hz.316326.xyz/gtpggllyys.html

stop)  echo "停止" ;;
来源：http://hz.mhx1999.top/gthstuignj.html

*)     echo "未知命令" ;;
来源：http://hz.sweek.top/gtcwjimryo.html

esac
来源：http://hz.aibaodan.cn/gtkxzcfroo.html

[R12] for 遍历文件
来源：http://hz.52xcode.cn/gtzizeuzmk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.0kj1m.cn/gtfjmexpco.html

[R13] for 计数循环
来源：http://hz.ehwqpu.com/gtpblyvihr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cqqwz.cn/gtpqnocfnj.html

[R14] C 风格 for
来源：http://hz.jinqigfzy.top/gtbulzmsgb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.aizwys.cn/gtyortdsry.html

[R15] while 逐行读文件
来源：http://hz.ivvv.top/gtkfqjiait.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daxiang520.top/gtfcbatsfg.html

[R16] until 等待条件
来源：http://hz.pycfn.com/gtqppcfudi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gogol.net.cn/gtfkwnnqcv.html

[R17] 数组定义与取值
来源：http://hz.yj202588.top/gtdxcpfkba.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yuxming.cn/gtetndilbi.html

[R18] 遍历数组
来源：http://hz.xuanzx.com/gtmoqysdoh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenzaomai.com/gtkxozeory.html

[R19] 数组长度
来源：http://hz.aizwys.cn/gtcxqtkher.html

echo "${#arr[@]}"
来源：http://hz.0kj1m.cn/gtpmwdpmcq.html

[R20] 关联数组（字典）
来源：http://hz.zhixingplan.top/gtoxsnkxta.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangshuangyany.cn/gtymmvcfor.html

[R21] 字符串长度
来源：http://hz.yuxming.cn/gtubfazaax.html

echo "${#s}"
来源：http://hz.52xcode.cn/gtdyhppjbi.html

[R22] 截取子串
来源：http://hz.xinyue.icu/gtsuyaszew.html

echo "${s:0:5}"
来源：http://hz.smart0.xyz/gtcnzuiqoi.html

[R23] 字符串替换
来源：http://hz.smart0.xyz/gtpqeckdgk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.kuanghao11.cn/gtjusmvcia.html

[R24] 大小写转换
来源：http://hz.gzhubu.top/gtrzotjqre.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.haohaochexian.top/gtoapqwvry.html

[R25] 去后缀 / 去前缀
来源：http://hz.zycfv.cn/gtgisjmgtt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tian-w.cn/gtzmpnniyh.html

[R26] 命令替换
来源：http://hz.zycfv.cn/gtmvdeoete.html

now=$(date +%F); echo "$now"
来源：http://hz.zhijiandao.cn/gtjeydpnma.html

[R27] 算术展开
来源：http://hz.yj20258.top/gtipakzyrj.html

echo $((1 + 2 * 3))
来源：http://hz.smart0.xyz/gttfweucik.html

[R28] 浮点运算
来源：http://hz.jiagoushi.top/gtlncokncj.html

echo "scale=2; 10/3" | bc
来源：http://hz.xuanzx.com/gtfgatzetk.html

[R29] 定义函数
来源：http://hz.jiagoushi.top/gtpbrdupse.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yanxiufei.cn/gtdxjaaedg.html

[R30] 函数返回状态码
来源：http://hz.aibaodan.cn/gtctdhpeoy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yongpay.top/gtacfpzxbx.html

[R31] 局部变量
来源：http://hz.aibaodan.cn/gtofdkwear.html

f() { local x=1; echo "$x"; }
来源：http://hz.sweek.top/gtcqzgzbmo.html

[R32] 参数个数校验
来源：http://hz.nanxuanxn.top/gtsjwmxblv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxuanxn.top/gtgfwvywdh.html

[R33] 捕获错误并提示行号
来源：http://hz.jinghuilouyu.cn/gtuvlixoxr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.bjfxy.top/gtnuojzqxw.html

[R34] 退出时清理
来源：http://hz.daria6918.cn/gtbcljizqz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuanzhike.top/gtwzucesfs.html

[R35] 后台执行并等待
来源：http://hz.chenzaomai.com/gtxfbwldog.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj20258888.top/gtmvjziljl.html

[R36] 并发执行多个任务
来源：http://hz.jqgfzy.top/gtjmyzvyeh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.smart0.xyz/gtsqckkxjn.html

[R37] 把输出赋给变量
来源：http://hz.zhiwuduotai.top/gtbldnmscs.html

files=$(ls -1)
来源：http://hz.nanxuanxn.top/gtbwlwbuoa.html

[R38] 管道串联
来源：http://hz.hfpthk.cn/gtvvfyhtqk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.pycfn.com/gtljnqjxqv.html

[R39] 重定向标准输出与错误
来源：http://hz.shuidangran.top/gtddzreyjl.html

cmd > out.log 2>&1
来源：http://hz.jyoumei.cn/gtwxunzwgk.html

[R40] 追加写日志
来源：http://hz.havefunace.top/gtgntbdpiu.html

echo "log" >> out.log
来源：http://hz.yj20258.top/gtnqelkbom.html

[R41] 丢弃输出
来源：http://hz.yanxiufei.cn/gtcbqgkifq.html

cmd >/dev/null 2>&1
来源：http://hz.52xcode.cn/gtdsgnluht.html

[R42] 输入重定向
来源：http://hz.zhixingplan.top/gtkirwommm.html

wc -l < a.txt
来源：http://hz.tian-w.cn/gtrrveuroc.html

[R43] 按名字查找文件
来源：http://hz.xinyue.icu/gtbvclfltj.html

find . -name "*.log" -type f
来源：http://hz.jqgfzy.top/gtkelvobtd.html

[R44] 按修改时间查找
来源：http://hz.c1oappe.top/gterficrzx.html

find . -mtime -7 -type f
来源：http://hz.hysaishi.cn/gtbdjlmwxo.html

[R45] 批量删除
来源：http://hz.hysaishi.cn/gthlrradbo.html

find . -name "*.tmp" -delete
来源：http://hz.chenjidiqi.icu/gtuhhkdvyu.html

[R46] 递归替换文件内容
来源：http://hz.yj202588.top/gtzcxhyvvn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinyuanbaomall.cn/gtoypykefh.html

[R47] sed 单行替换
来源：http://hz.yangfankeji.com/gtgnovyhee.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nwbrower.top/gtzpsqwbwm.html

[R48] awk 取指定列
来源：http://hz.cdnleiting.top/gtamlrcmxy.html

awk '{print $1, $3}' a.txt
来源：http://hz.ybcxt.top/gtaskctaas.html

[R49] awk 带条件
来源：http://hz.cqqwz.cn/gtpuwekrvi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.haohaochexian.top/gttkxrerwf.html

[R50] awk 求和
来源：http://hz.bjfxy.top/gtcndjmrsa.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj202588.top/gtplmaphtb.html

[R51] 排序去重取前几
来源：http://hz.jinghuilouyu.cn/gtrdybrpyr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tianlin.xyz/gtaclcqfwp.html

[R52] 统计行数
来源：http://hz.0kj1m.cn/gtwelhierh.html

wc -l a.txt
来源：http://hz.ydzc1.top/gtwvebptkl.html

[R53] 查看文件头与实时尾
来源：http://hz.zdqjudy.top/gtsotwonwt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shzxlz.cn/gtfjwhxxro.html

[R54] 比较两个文件
来源：http://hz.vqdsnc.cn/gthjmhtpho.html

diff a.txt b.txt
来源：http://hz.ivvv.top/gthhflpbgo.html

[R55] 压缩与解压
来源：http://hz.nwbrower.top/gtiewdkxeh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.quarkkingdee.top/gtxphfnpyo.html

[R56] 远程拷贝
来源：http://hz.shzxlz.cn/gtdbhpnxmm.html

scp file user@host:/path/
来源：http://hz.jinghuilouyu.cn/gtlinstlyi.html

[R57] 远程执行命令
来源：http://hz.jinqigfzy.top/gtunbwbudf.html

ssh user@host 'uptime'
来源：http://hz.chenzaomai.com/gtdrpdappx.html

[R58] 下载文件
来源：http://hz.mhx1999.top/gtkvlvhbny.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sweek.top/gtsqrhtmwu.html

[R59] 发 POST JSON
来源：http://hz.daria6918.cn/gtvywsuytx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gotoacloud.top/gtinarimbb.html

[R60] 只看 HTTP 状态码
来源：http://hz.gzhubu.top/gtjoghujgl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhongyouzk.top/gtgpvmjthx.html

[R61] 磁盘占用
来源：http://hz.nanxinkj.top/gtrlipfxdt.html

df -h;  du -sh *
来源：http://hz.gzhubu.top/gthoqghehe.html

[R62] 找最占空间的文件
来源：http://hz.xuanzx.com/gtavbrhndk.html

du -ah . | sort -rh | head -10
来源：http://hz.chenjidiqi.icu/gtapgishmm.html

[R63] 内存与进程
来源：http://hz.jianghu66.top/gtvzmbstdd.html

free -h;  ps aux | grep nginx
来源：http://hz.sysykeji.top/gtplkyjvre.html

[R64] 结束进程
来源：http://hz.nanxuanxn.top/gtmowptrnt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ybcxt.top/gtrtmcfoqf.html

[R65] 查看端口占用
来源：http://hz.chenjidiqi.icu/gtaenkognx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.meibo888.top/gtxqusfnzh.html

[R66] 定时任务
来源：http://hz.yonumen.top/gtkajukynu.html

crontab -e;  crontab -l
来源：http://hz.ydzc1.top/gtjwahvfoe.html

[R67] 生成随机十六进制串
来源：http://hz.zdqjudy.top/gthhuzticb.html

openssl rand -hex 16
来源：http://hz.jqgfzy.top/gtgritthsj.html

[R68] 计算文件校验值
来源：http://hz.yuxming.cn/gtixqpnyxp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.feifeiyinyue.top/gtvsifsnlr.html

[R69] 生成随机密码
来源：http://hz.ppjwa.cn/gtbeayoqvz.html

head -c 16 /dev/urandom | base64
来源：http://hz.wangdashe.top/gtwocmvfak.html

[R70] 时间戳与互转
来源：http://hz.iojbl.cn/gtwimygjnx.html

date +%s;  date -d @1700000000
来源：http://hz.sxryk.cn/gthyubyxlu.html

[R71] 日期格式化
来源：http://hz.zhixingplan.top/gtqbjoxsue.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuetiantiany.cn/gtmvezhfxa.html

[R72] 等待端口就绪
来源：http://hz.wangshuangyany.cn/gtwtutcgoz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yuxming.cn/gtfiohjayk.html

[R73] 分割大日志
来源：http://hz.jyoumei.cn/gtlfwpukag.html

split -l 1000 big.log part_
来源：http://hz.cucudq.cn/gteeqdbrnq.html

[R74] 批量重命名
来源：http://hz.snrcjt.cn/gtllcuaujj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xziqi.cn/gtotvyfqzg.html

[R75] 导出环境变量
来源：http://hz.zdqjudy.top/gtbnkawjpg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.fzhhl.top/gthjykxfke.html

[R76] 使用临时文件
来源：http://hz.birdmap.top/gtygjkwzly.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gthjznrlfl.html

[R77] 读取用户输入
来源：http://hz.zhiwuduotai.top/gtlqtvaqlm.html

read -rp "请输入: " ans
来源：http://hz.daria6918.cn/gtwtdqtfvv.html

[R78] 交互式菜单
来源：http://hz.xziqi.cn/gtkykwvrob.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangdashe.top/gtkdvskupl.html

[R79] 解析命令行选项
来源：http://hz.jlsjyb.cn/gtwsqxumxs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zdqjudy.top/gtqeukllfn.html

[R80] 查看脚本执行耗时
来源：http://hz.0kj1m.cn/gtgmakfhss.html

time ./run.sh
来源：http://hz.haohaochexian.top/gtidbknukx.html

================================================================================
来源：http://hz.cashguo.top/gtpooqmucl.html

S. C / C++ 专题
来源：http://hz.tanke756.top/gtwwbmyfku.html

================================================================================
来源：http://hz.dianchejie.cn/gtqiroakdr.html

[S01] C：Hello World
来源：http://hz.chenzaomai.com/gtmybwiuna.html

#include <stdio.h>
来源：http://hz.gotoacloud.top/gtyblmogni.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xziqi.cn/gtndbtkzce.html

[S02] C：变量与格式化输出
来源：http://hz.xuetiantiany.cn/gtsavhahad.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuxming.cn/gtrwfesbeo.html

[S03] C：读入整数
来源：http://hz.yanxiufei.cn/gtcnqkgqjd.html

int x; scanf("%d", &x);
来源：http://hz.yonumen.top/gttxwlnufj.html

[S04] C：字符串复制
来源：http://hz.aizwys.cn/gtdmdnuqpg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gogol.net.cn/gtapuqlldv.html

[S05] C：字符串长度
来源：http://hz.jianghu66.top/gtbespmsij.html

strlen(s)
来源：http://hz.nwbrower.top/gtzugzzldn.html

[S06] C：字符串比较
来源：http://hz.yuxming.cn/gtmyfyinia.html

strcmp(a, b) == 0
来源：http://hz.yongpay.top/gtbsbrboxh.html

[S07] C：数组遍历求和
来源：http://hz.yj202588.top/gtrdhzpziu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.pengpengdd.cyou/gtungtmbmj.html

[S08] C：动态内存分配与释放
来源：http://hz.shzxlz.cn/gtxvzrnrhp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zdqjudy.top/gtuireselo.html

[S09] C：结构体定义与初始化
来源：http://hz.bjfxy.top/gtsimhumko.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cucudq.cn/gtkhkjqlbd.html

[S10] C：指针与解引用
来源：http://hz.zhixingplan.top/gtjmzfaqbw.html

int *p = &a;  *p = 5;
来源：http://hz.zhongyouzk.top/gtbqjhlcjy.html

[S11] C：逐行读文件
来源：http://hz.nanxinkj.top/gtlkyvfwlj.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.daxiang520.top/gtdctceomi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hammf.cn/gtwuhgqsnd.html

fclose(f);
来源：http://hz.quarkkingdee.top/gthniiwebw.html

[S12] C：写文件
来源：http://hz.hnqzz.top/gtayxtyqzp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jiagoushi.top/gtapkprmjl.html

[S13] C：宏定义
来源：http://hz.yj20258.top/gtvrqwhbgt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gtnvecaczx.html

[S14] C：枚举
来源：http://hz.jlsjyb.cn/gttiktmxaw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.bjfxy.top/gtmoaozojd.html

[S15] C：类型转换
来源：http://hz.pengpengdd.cyou/gtzxevplli.html

(double) a / b
来源：http://hz.zycfv.cn/gtafhmbbsw.html

[S16] C：位操作置位
来源：http://hz.zhixingplan.top/gtdysfgqjk.html

x |= (1 << 3);
来源：http://hz.yuanzhike.top/gtcwzjipxl.html

[S17] C：安全拼接字符串
来源：http://hz.jinqigufen.top/gtlxkjuzkj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.vqdsnc.cn/gtrpeobkuv.html

[S18] C：命令行参数
来源：http://hz.zhiwuduotai.top/gtrmlwyjuq.html

int main(int argc, char **argv)
来源：http://hz.tanke756.top/gtuaycdffu.html

[S19] C：快速排序
来源：http://hz.andypj.xyz/gtxrkatcnq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtfjdihiwx.html

[S20] C：二分查找
来源：http://hz.jinqigfzy.top/gtllodwhur.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jqgufenzy.top/gtevmjdqyh.html

[S21] C：字符类别判断
来源：http://hz.dashuyun.cn/gtjknlwagl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xuetiantiany.cn/gtfxozolwe.html

[S22] C：字符串转数字
来源：http://hz.jqgfzy.top/gtefdomkcq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.c1oappe.top/gtbkghulye.html

[S23] C：随机数
来源：http://hz.guowangkeji.top/gtkogsgqzf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangshuangyany.cn/gtijxrngst.html

[S24] C：获取本地时间
来源：http://hz.redwolf501.top/gtcmnzoact.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinqigfzy.top/gtjinuszfr.html

[S25] C：内存拷贝
来源：http://hz.andypj.xyz/gtmbxzotit.html

memcpy(dst, src, n);
来源：http://hz.yj20258.top/gtwtjkwliv.html

[S26] C：内存清零
来源：http://hz.0kj1m.cn/gtunlawhko.html

memset(a, 0, sizeof a);
来源：http://hz.yvedp.cn/gtroaiuwor.html

[S27] C：定义常量
来源：http://hz.quarkkingdee.top/gthjvwzqmg.html

const double PI = 3.14159;
来源：http://hz.dianchejie.cn/gtdzbrrttv.html

[S28] C：静态变量
来源：http://hz.ehwqpu.com/gtuolcvbuo.html

static int counter = 0;
来源：http://hz.52xcode.cn/gtmonrdnli.html

[S29] C：变参函数
来源：http://hz.aizwys.cn/gtcabqkuhg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yj20258888.top/gtplhvwrsc.html

[S30] C：头文件保护
来源：http://hz.9152youxi.cn/gtkdtridnq.html

#ifndef X_H
来源：http://hz.iojbl.cn/gtdjdaxehr.html

#define X_H
来源：http://hz.jyoumei.cn/gtzmsqabxb.html

#endif
来源：http://hz.jqgufenzy.top/gtvdknuovy.html

[S31] C++：Hello World
来源：http://hz.daxiang520.top/gtosntnlox.html

#include <iostream>
来源：http://hz.yueranfly.top/gtwwvhjwit.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ydzc1.top/gtuvuusauh.html

[S32] C++：字符串
来源：http://hz.tianlin.xyz/gtoofipies.html

std::string s = "hi";  s += "!";
来源：http://hz.jianghu66.top/gtfbwzixvn.html

[S33] C++：vector 增删
来源：http://hz.jqgufenzy.top/gtvziavbtm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yanxiufei.cn/gtkjlywghs.html

[S34] C++：遍历 vector
来源：http://hz.yuanzhike.top/gtkjhyrtev.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jlsjyb.cn/gttocrhflq.html

[S35] C++：map
来源：http://hz.hammf.cn/gtfxvwdcim.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gtvswcawvv.html

[S36] C++：unordered_map
来源：http://hz.smart0.xyz/gtnjlfciub.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yonumen.top/gtrqeizcep.html

[S37] C++：set
来源：http://hz.ydjk.org.cn/gtlfvnmhrr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yanxiufei.cn/gtuqgsekfb.html

[S38] C++：排序
来源：http://hz.ivvv.top/gtqslsetml.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxinkj.top/gtwksopxne.html

[S39] C++：自定义比较器排序
来源：http://hz.svipenyu.cn/gtsyadqfxb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhongyouzk.top/gttpckuxuc.html

[S40] C++：查找元素
来源：http://hz.0kj1m.cn/gtvqcrturq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.feifeiyinyue.top/gtxtslosin.html

[S41] C++：类与构造函数
来源：http://hz.birdmap.top/gtmvhsvuzv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhiwuduotai.top/gtkphlgjji.html

[S42] C++：继承与虚函数
来源：http://hz.pycfn.com/gttyjrhbes.html

class B : public Base { public: void f() override {} };
来源：http://hz.bjfxy.top/gthjnfoich.html

[S43] C++：智能指针
来源：http://hz.hnqzz.top/gtlocksjvw.html

auto p = std::make_unique<int>(5);
来源：http://hz.ybcxt.top/gthjctvzzg.html

[S44] C++：引用传参
来源：http://hz.sxryk.cn/gtuucgjhmw.html

void inc(int &x) { ++x; }
来源：http://hz.ywan-chungtsiang.top/gtfowurklg.html

[S45] C++：lambda
来源：http://hz.sweek.top/gtzcxeekjf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhiwuduotai.top/gtdmtneamj.html

[S46] C++：函数模板
来源：http://hz.xuanzx.com/gtyrpnrjis.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhijiandao.cn/gtofktaueu.html

[S47] C++：结构化绑定遍历
来源：http://hz.hongshengwenyu.top/gtpxpjwwlk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.daxiang520.top/gtanqicgfe.html

[S48] C++：逐行读文件
来源：http://hz.jiagoushi.top/gtglhplnbq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.pycfn.com/gtrsboacex.html

while (std::getline(in, line)) { }
来源：http://hz.hammf.cn/gtidzrfiwd.html

[S49] C++：写文件
来源：http://hz.wangdashe.top/gtyuixpcjc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.9152youxi.cn/gtfrqnhvig.html

[S50] C++：格式化数字
来源：http://hz.shzxlz.cn/gtsiwgztvo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.c1oappe.top/gtupsnpygd.html

[S51] C++：显式类型转换
来源：http://hz.jiagoushi.top/gtklxjgrze.html

static_cast<double>(a) / b
来源：http://hz.wangshuangyany.cn/gtzjllxexl.html

[S52] C++：const 与 noexcept
来源：http://hz.jiagoushi.top/gteeccmxfn.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtnqnsosly.html

[S53] C++：移动语义
来源：http://hz.xinyue.icu/gttysgugsn.html

std::vector<int> w = std::move(v);
来源：http://hz.gogol.net.cn/gthzdkdzjz.html

[S54] C++：异常处理
来源：http://hz.smart0.xyz/gtgnvlmfmb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jqgufenzy.top/gtvppkmfhn.html

[S55] C++：结构化绑定
来源：http://hz.jinqigufen.top/gttzhmziep.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.redwolf501.top/gtokakekpr.html

[S56] C++：optional
来源：http://hz.yongpay.top/gterrqalgt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hnqzz.top/gtmjctomhu.html

[S57] C++：编译期常量
来源：http://hz.52xcode.cn/gtkpohdajl.html

constexpr int N = 10;
来源：http://hz.yvedp.cn/gtvhpnarxy.html

[S58] C++：命名空间
来源：http://hz.0kj1m.cn/gtyhfchjbs.html


<!-- 参考信息 -->