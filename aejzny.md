代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://hz.yvedp.cn/gtfnxmrlul.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj20258.top/gtmzbtkyom.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ppjwa.cn/gtubqcggks.html

[Q89] 判断表是否存在
来源：http://hz.jyoumei.cn/gthemovuup.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hywenlv.cn/gtvwderyzf.html

[Q90] 生成序号列
来源：http://hz.xuetiantiany.cn/gttafxpewf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fzhhl.top/gturqhicss.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtdccfxwen.html

R. Bash 专题
来源：http://hz.guannengcc.top/gtdduntuxm.html

================================================================================
来源：http://hz.smart0.xyz/gtbodyzazg.html

[R01] shebang 与严格模式
来源：http://hz.ppjwa.cn/gtgscrqckm.html

#!/usr/bin/env bash
来源：http://hz.yj20258888.top/gtfudmmcej.html

set -euo pipefail
来源：http://hz.aizwys.cn/gtpcfidqxb.html

[R02] 变量赋值与使用
来源：http://hz.zhoulong.xyz/gtggbjkkux.html

name="Tom"; echo "$name"
来源：http://hz.aibaodan.cn/gthltdzjvj.html

[R03] 只读变量
来源：http://hz.ywan-chungtsiang.top/gtzejobsgw.html

readonly PI=3.14
来源：http://hz.daria6918.cn/gtqyhjjbfl.html

[R04] 位置参数
来源：http://hz.yj20258888.top/gtprhqresh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinyuanbaomall.cn/gtmcwmgegt.html

[R05] 参数默认值
来源：http://hz.smart0.xyz/gtyaomfjxz.html

name="${1:-default}"
来源：http://hz.zdqjudy.top/gtqgtrtkfe.html

[R06] 判断命令是否存在
来源：http://hz.haohaochexian.top/gtajegvdxs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shuidangran.top/gtvvvuujgr.html

[R07] if 判断文件
来源：http://hz.yj202588.top/gtajfymqzz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj202588.top/gthhilsihf.html

[R08] 数值比较
来源：http://hz.jlsjyb.cn/gtdsjhsjpp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tanke756.top/gtuiezsalj.html

[R09] 字符串比较
来源：http://hz.iojbl.cn/gtfizofdfl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yuxming.cn/gtltxollav.html

[R10] 正则匹配
来源：http://hz.tianlin.xyz/gtdqeuwksc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.aizwys.cn/gtxrnjkspi.html

[R11] case 多分支
来源：http://hz.nanxinkj.top/gtztyfofnh.html

case "$1" in
来源：http://hz.bjfxy.top/gtunkhyjxj.html

start) echo "启动" ;;
来源：http://hz.dashuyun.cn/gtoawllspa.html

stop)  echo "停止" ;;
来源：http://hz.jinqigfzy.top/gtkclimbxt.html

*)     echo "未知命令" ;;
来源：http://hz.redwolf501.top/gtzoqznkwy.html

esac
来源：http://hz.gzhubu.top/gtkautnbmb.html

[R12] for 遍历文件
来源：http://hz.guannengcc.top/gttcixxaha.html

for f in *.txt; do echo "$f"; done
来源：http://hz.aizwys.cn/gtmpkalqkw.html

[R13] for 计数循环
来源：http://hz.jiagoushi.top/gttccvgiud.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.9152youxi.cn/gtvkldomgd.html

[R14] C 风格 for
来源：http://hz.gzhubu.top/gtyvfadzeq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xziqi.cn/gttmfbwjtb.html

[R15] while 逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtigvjisdy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigfzy.top/gtzqzebpaz.html

[R16] until 等待条件
来源：http://hz.jqgufenzy.top/gtotvivtvc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenzaomai.com/gtminovwik.html

[R17] 数组定义与取值
来源：http://hz.shuidangran.top/gtodunqrky.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jlsjyb.cn/gtqhgamrbx.html

[R18] 遍历数组
来源：http://hz.wangdashe.top/gtkpvglqll.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgfzy.top/gtivbixxsb.html

[R19] 数组长度
来源：http://hz.jinqigfzy.top/gtcwtpbmqc.html

echo "${#arr[@]}"
来源：http://hz.yongpay.top/gthnysdmng.html

[R20] 关联数组（字典）
来源：http://hz.wangshuangyany.cn/gtifpxhtxo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinqigfzy.top/gtnxlauxhn.html

[R21] 字符串长度
来源：http://hz.bjfxy.top/gttkjkujfg.html

echo "${#s}"
来源：http://hz.daxiang520.top/gtdtqvxqbl.html

[R22] 截取子串
来源：http://hz.ppjwa.cn/gtmpdmbafm.html

echo "${s:0:5}"
来源：http://hz.hnqzz.top/gtuvjdtsaj.html

[R23] 字符串替换
来源：http://hz.52xcode.cn/gteyilaehp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shuidangran.top/gtwhnkpkhi.html

[R24] 大小写转换
来源：http://hz.meibo888.top/gtxpwsgglv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jqgufenzy.top/gtmjkuesat.html

[R25] 去后缀 / 去前缀
来源：http://hz.yonumen.top/gtyxhufuda.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhijiandao.cn/gtkrhsilfz.html

[R26] 命令替换
来源：http://hz.yvedp.cn/gtupeblrsq.html

now=$(date +%F); echo "$now"
来源：http://hz.jianghu66.top/gttlsffdit.html

[R27] 算术展开
来源：http://hz.aibaodan.cn/gtfijuzpuk.html

echo $((1 + 2 * 3))
来源：http://hz.yuxming.cn/gtuvlnfhmw.html

[R28] 浮点运算
来源：http://hz.yongpay.top/gtxcyudqga.html

echo "scale=2; 10/3" | bc
来源：http://hz.0kj1m.cn/gtqeglxrtp.html

[R29] 定义函数
来源：http://hz.gzhubu.top/gtkouvjxsk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cdnleiting.top/gtiozutgsr.html

[R30] 函数返回状态码
来源：http://hz.yonumen.top/gtvbhdiekf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.fzhhl.top/gtyilscfgl.html

[R31] 局部变量
来源：http://hz.smart0.xyz/gtavxjjtou.html

f() { local x=1; echo "$x"; }
来源：http://hz.jqgfzy.top/gtlkjpoqpy.html

[R32] 参数个数校验
来源：http://hz.ybcxt.top/gtkxyilnvq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhiwuduotai.top/gtyzyediek.html

[R33] 捕获错误并提示行号
来源：http://hz.tian-w.cn/gtxyzkomjn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhijiandao.cn/gthjgvihwl.html

[R34] 退出时清理
来源：http://hz.jinyuanbaomall.cn/gtzkbrbggp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtgvxkcvgl.html

[R35] 后台执行并等待
来源：http://hz.zhengqikj.top/gtvycxgqte.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhengqikj.top/gturvbegdq.html

[R36] 并发执行多个任务
来源：http://hz.jqgfzy.top/gtwoknkamy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yangfankeji.com/gtnfvzrsha.html

[R37] 把输出赋给变量
来源：http://hz.wangshuangyany.cn/gtaljsshkp.html

files=$(ls -1)
来源：http://hz.jiagoushi.top/gtxcoalpxd.html

[R38] 管道串联
来源：http://hz.shuidangran.top/gtlwpvqmvc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yuanzhike.top/gtfkrpbjkz.html

[R39] 重定向标准输出与错误
来源：http://hz.mhx1999.top/gtgxrrosfg.html

cmd > out.log 2>&1
来源：http://hz.quarkkingdee.top/gtwjkngkxb.html

[R40] 追加写日志
来源：http://hz.daria6918.cn/gtkeacammq.html

echo "log" >> out.log
来源：http://hz.daria6918.cn/gttebntkzv.html

[R41] 丢弃输出
来源：http://hz.nanxuanxn.top/gtrshurvvz.html

cmd >/dev/null 2>&1
来源：http://hz.cqqwz.cn/gtjueyglzh.html

[R42] 输入重定向
来源：http://hz.ywan-chungtsiang.top/gtumawpsbb.html

wc -l < a.txt
来源：http://hz.jiagoushi.top/gtdybjvfcd.html

[R43] 按名字查找文件
来源：http://hz.kuanghao11.cn/gtifvomude.html

find . -name "*.log" -type f
来源：http://hz.hongshengwenyu.top/gtqkqfjfmh.html

[R44] 按修改时间查找
来源：http://hz.sufxvd.cn/gtikwqacpv.html

find . -mtime -7 -type f
来源：http://hz.guowangkeji.top/gtbxtktsns.html

[R45] 批量删除
来源：http://hz.aizwys.cn/gtktyipzqx.html

find . -name "*.tmp" -delete
来源：http://hz.mhx1999.top/gtujiwqwft.html

[R46] 递归替换文件内容
来源：http://hz.kuanghao11.cn/gtclglthst.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.meibo888.top/gtklabgmzh.html

[R47] sed 单行替换
来源：http://hz.ehwqpu.com/gtvqqcohei.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cdnleiting.top/gthrzaoiuz.html

[R48] awk 取指定列
来源：http://hz.jqgfzy.top/gtplkhbyib.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj202588.top/gtvjvmxjiw.html

[R49] awk 带条件
来源：http://hz.sxryk.cn/gtvosygvdz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jqgufenzy.top/gtevdlputb.html

[R50] awk 求和
来源：http://hz.yangfankeji.com/gtsftejpmh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guannengcc.top/gtvjxpksgu.html

[R51] 排序去重取前几
来源：http://hz.yvedp.cn/gtvfvlixme.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.52xcode.cn/gtfrzndxhh.html

[R52] 统计行数
来源：http://hz.redwolf501.top/gtinjbnpug.html

wc -l a.txt
来源：http://hz.yj202588.top/gtsootaagx.html

[R53] 查看文件头与实时尾
来源：http://hz.shanyushiyangkeji.top/gtblrktuzl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dianchejie.cn/gttfmocxla.html

[R54] 比较两个文件
来源：http://hz.shzxlz.cn/gtucbuuphv.html

diff a.txt b.txt
来源：http://hz.zhijiandao.cn/gtrzopmwgq.html

[R55] 压缩与解压
来源：http://hz.ywan-chungtsiang.top/gtaaiwawfv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuetiantiany.cn/gtgpqioinv.html

[R56] 远程拷贝
来源：http://hz.yj202588.top/gtvhltipsj.html

scp file user@host:/path/
来源：http://hz.ehwqpu.com/gtedpqnwos.html

[R57] 远程执行命令
来源：http://hz.yuanzhike.top/gtziepyflk.html

ssh user@host 'uptime'
来源：http://hz.xylfe.cn/gtfxvqotvh.html

[R58] 下载文件
来源：http://hz.vqdsnc.cn/gtcvddxsyl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gotoacloud.top/gtrjgecayw.html

[R59] 发 POST JSON
来源：http://hz.hnqzz.top/gtkddakude.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangdashe.top/gtbipbfsji.html

[R60] 只看 HTTP 状态码
来源：http://hz.jyoumei.cn/gtwjsybbcp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xingfuxueyuan.xyz/gtaslgcvwr.html

[R61] 磁盘占用
来源：http://hz.zhijiandao.cn/gtujtmsaxl.html

df -h;  du -sh *
来源：http://hz.ivvv.top/gteuzpsjhq.html

[R62] 找最占空间的文件
来源：http://hz.feifeiyinyue.top/gtyyjeyimn.html

du -ah . | sort -rh | head -10
来源：http://hz.jinqigfzy.top/gtrrustsnk.html

[R63] 内存与进程
来源：http://hz.yuanzhike.top/gtrcicxpap.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxuanxn.top/gttcraynbz.html

[R64] 结束进程
来源：http://hz.xingfuxueyuan.xyz/gtobnphggh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jqgufenzy.top/gtlkurjlgy.html

[R65] 查看端口占用
来源：http://hz.xinyue.icu/gtmjvwedlu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sweek.top/gtrzwgrjwq.html

[R66] 定时任务
来源：http://hz.sufxvd.cn/gtmfrbnjqv.html

crontab -e;  crontab -l
来源：http://hz.jinqigufen.top/gtarlpiitc.html

[R67] 生成随机十六进制串
来源：http://hz.jinyuanbaomall.cn/gtjhjgelce.html

openssl rand -hex 16
来源：http://hz.dianchejie.cn/gtxsxiyxbj.html

[R68] 计算文件校验值
来源：http://hz.shangyingyoupin.top/gttrawwace.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ywan-chungtsiang.top/gtygjuwopl.html

[R69] 生成随机密码
来源：http://hz.vqdsnc.cn/gtgwmbvbfx.html

head -c 16 /dev/urandom | base64
来源：http://hz.gogol.net.cn/gtijmdrmdc.html

[R70] 时间戳与互转
来源：http://hz.yueranfly.top/gtgvvzaylc.html

date +%s;  date -d @1700000000
来源：http://hz.kuanghao11.cn/gtnlajqlrr.html

[R71] 日期格式化
来源：http://hz.iojbl.cn/gtozfoypsb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hysaishi.cn/gtxdotlweu.html

[R72] 等待端口就绪
来源：http://hz.jinghuilouyu.cn/gtilglmotc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.316326.xyz/gtcsirirwr.html

[R73] 分割大日志
来源：http://hz.iojbl.cn/gtsprtwwng.html

split -l 1000 big.log part_
来源：http://hz.jinghuilouyu.cn/gtnvbycfld.html

[R74] 批量重命名
来源：http://hz.xingfuxueyuan.xyz/gtxtqzuqzj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tanke756.top/gtvvsxowhx.html

[R75] 导出环境变量
来源：http://hz.zhongyouzk.top/gtcfdxenvu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xuetiantiany.cn/gtbgvwmfvb.html

[R76] 使用临时文件
来源：http://hz.wangdashe.top/gtfjhjgpvn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gtrsjkfllj.html

[R77] 读取用户输入
来源：http://hz.dashuyun.cn/gttkhwnkga.html

read -rp "请输入: " ans
来源：http://hz.daria6918.cn/gtmmerufol.html

[R78] 交互式菜单
来源：http://hz.tian-w.cn/gtqejvsffp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jianghu66.top/gtvukfuvpy.html

[R79] 解析命令行选项
来源：http://hz.yonumen.top/gtdnqrphfe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhixingplan.top/gtisjnmscg.html

[R80] 查看脚本执行耗时
来源：http://hz.yj202588.top/gtvjrtkiph.html

time ./run.sh
来源：http://hz.chenjidiqi.icu/gtdukzduli.html

================================================================================
来源：http://hz.yvedp.cn/gthmgsidkx.html

S. C / C++ 专题
来源：http://hz.gzhubu.top/gtqwwhuvgs.html

================================================================================
来源：http://hz.zdqjudy.top/gtteeeusno.html

[S01] C：Hello World
来源：http://hz.redwolf501.top/gtwaiovgvl.html

#include <stdio.h>
来源：http://hz.xylfe.cn/gtkaelptab.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.havefunace.top/gtnussyxse.html

[S02] C：变量与格式化输出
来源：http://hz.yj20258.top/gtpsudjnlr.html

int a = 10; printf("%d\n", a);
来源：http://hz.gogol.net.cn/gtempsopiw.html

[S03] C：读入整数
来源：http://hz.jyoumei.cn/gtpvyfvsgm.html

int x; scanf("%d", &x);
来源：http://hz.jinghuilouyu.cn/gtfdgengvd.html

[S04] C：字符串复制
来源：http://hz.yongpay.top/gtkplfnbfe.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shzxlz.cn/gtmcwquyej.html

[S05] C：字符串长度
来源：http://hz.jyoumei.cn/gtlavqiyfp.html

strlen(s)
来源：http://hz.xylfe.cn/gtyqflgcaa.html

[S06] C：字符串比较
来源：http://hz.yonumen.top/gtzdcarvrg.html

strcmp(a, b) == 0
来源：http://hz.0kj1m.cn/gtspppfjvt.html

[S07] C：数组遍历求和
来源：http://hz.zycfv.cn/gtejlhdevx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jyoumei.cn/gtqxoxdsin.html

[S08] C：动态内存分配与释放
来源：http://hz.vqdsnc.cn/gtqgwadtrh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.wangshuangyany.cn/gtyxloyikj.html

[S09] C：结构体定义与初始化
来源：http://hz.wangshuangyany.cn/gttphshjoa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.bjfxy.top/gtinhkfhkj.html

[S10] C：指针与解引用
来源：http://hz.svipenyu.cn/gtypdkltjp.html

int *p = &a;  *p = 5;
来源：http://hz.ydzc1.top/gtbwbuqbjj.html

[S11] C：逐行读文件
来源：http://hz.meibo888.top/gtpguwyiqr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jiagoushi.top/gtojtbfqge.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenzaomai.com/gtfckdeznp.html

fclose(f);
来源：http://hz.dashuyun.cn/gtmkgrxbxl.html

[S12] C：写文件
来源：http://hz.jinqigfzy.top/gtfsajdrne.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenzaomai.com/gtuifhllci.html

[S13] C：宏定义
来源：http://hz.hywenlv.cn/gtdykzkpld.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhaomingkeji.xyz/gtntiaoqdi.html

[S14] C：枚举
来源：http://hz.havefunace.top/gtthusqiqb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yongpay.top/gtyxbzeuoh.html

[S15] C：类型转换
来源：http://hz.cqqwz.cn/gtooirchns.html

(double) a / b
来源：http://hz.quarkkingdee.top/gtbgmareae.html

[S16] C：位操作置位
来源：http://hz.gzhubu.top/gtoybavxry.html

x |= (1 << 3);
来源：http://hz.daria6918.cn/gtxjipzxkq.html

[S17] C：安全拼接字符串
来源：http://hz.ivvv.top/gtnjrmluun.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.meibo888.top/gtwtsbhnyp.html

[S18] C：命令行参数
来源：http://hz.316326.xyz/gtekycxtrx.html

int main(int argc, char **argv)
来源：http://hz.meibo888.top/gtuowxouhw.html

[S19] C：快速排序
来源：http://hz.guannengcc.top/gtqufohswd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jqgufenzy.top/gtmqnlpdna.html

[S20] C：二分查找
来源：http://hz.jyoumei.cn/gthmibuqzd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.iojbl.cn/gtzcxuvsax.html

[S21] C：字符类别判断
来源：http://hz.yj20258888.top/gtbqxfcvre.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinqigfzy.top/gtmslkpdrw.html

[S22] C：字符串转数字
来源：http://hz.xingfuxueyuan.xyz/gtijtzupsc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.aibaodan.cn/gtpybxggnf.html

[S23] C：随机数
来源：http://hz.mhx1999.top/gtkcyxpzyx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.fzhhl.top/gtxmdfdstx.html

[S24] C：获取本地时间
来源：http://hz.jinghuilouyu.cn/gtponypzlp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.52xcode.cn/gtfvnchmzm.html

[S25] C：内存拷贝
来源：http://hz.wangdashe.top/gtccdcbjsu.html

memcpy(dst, src, n);
来源：http://hz.xuanzx.com/gtxqjjqyel.html

[S26] C：内存清零
来源：http://hz.9152youxi.cn/gtunxyjmsu.html

memset(a, 0, sizeof a);
来源：http://hz.sxryk.cn/gtvjhbtdnt.html

[S27] C：定义常量
来源：http://hz.zhaomingkeji.xyz/gtknpskmgj.html

const double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtacoctrzl.html

[S28] C：静态变量
来源：http://hz.gaohongyu789.top/gtpivgxbuk.html

static int counter = 0;
来源：http://hz.jlsjyb.cn/gtiloizpdo.html

[S29] C：变参函数
来源：http://hz.wangdashe.top/gtsrpuydbx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hammf.cn/gtposcxnjs.html

[S30] C：头文件保护
来源：http://hz.zhaomingkeji.xyz/gtjfnyjrwn.html

#ifndef X_H
来源：http://hz.hywenlv.cn/gtwkoxkxsh.html

#define X_H
来源：http://hz.guowangkeji.top/gtkvtcrslz.html

#endif
来源：http://hz.chenjidiqi.icu/gtutancfjw.html

[S31] C++：Hello World
来源：http://hz.redwolf501.top/gtioeyxyds.html

#include <iostream>
来源：http://hz.wangdashe.top/gtvodqcjne.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuetiantiany.cn/gtoqthwoqw.html

[S32] C++：字符串
来源：http://hz.kuanghao11.cn/gtgjgthkid.html

std::string s = "hi";  s += "!";
来源：http://hz.zhiwuduotai.top/gtohpkccfa.html

[S33] C++：vector 增删
来源：http://hz.aibaodan.cn/gtpxhmgsuh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhongyouzk.top/gtusccgkax.html

[S34] C++：遍历 vector
来源：http://hz.hnxiangtu.top/gtvgjfdvnw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenzaomai.com/gtkhpvsjye.html

[S35] C++：map
来源：http://hz.yanxiufei.cn/gtwqtwabmi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gttvgntcck.html

[S36] C++：unordered_map
来源：http://hz.ppjwa.cn/gtkbgjjyog.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.andypj.xyz/gtzbnrqjqc.html

[S37] C++：set
来源：http://hz.c1oappe.top/gtuyjgfzfp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.wangshuangyany.cn/gtdgzaesir.html

[S38] C++：排序
来源：http://hz.gzhubu.top/gtivaheswy.html

std::sort(v.begin(), v.end());
来源：http://hz.pengpengdd.cyou/gtquwvxtcm.html

[S39] C++：自定义比较器排序
来源：http://hz.yongpay.top/gtrnonzwnk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinghuilouyu.cn/gtiegcwlqe.html

[S40] C++：查找元素
来源：http://hz.zhijiandao.cn/gtyqcxtucm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhongyouzk.top/gtolkjdxiw.html

[S41] C++：类与构造函数
来源：http://hz.zhengqikj.top/gtteqyuvyv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gogol.net.cn/gtckqcvgdn.html

[S42] C++：继承与虚函数
来源：http://hz.snrcjt.cn/gtboqxifnt.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhixingplan.top/gtcegttpoh.html

[S43] C++：智能指针
来源：http://hz.xinyue.icu/gttculaknx.html

auto p = std::make_unique<int>(5);
来源：http://hz.snrcjt.cn/gtsgqfgjun.html

[S44] C++：引用传参
来源：http://hz.meibo888.top/gtevadyokg.html

void inc(int &x) { ++x; }
来源：http://hz.shuidangran.top/gtdswhjkxu.html

[S45] C++：lambda
来源：http://hz.gotoacloud.top/gtfeveanjf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhoulong.xyz/gtfwihfgpg.html

[S46] C++：函数模板
来源：http://hz.wangshuangyany.cn/gtjvixaeqw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xuanzx.com/gtybgdnmrn.html

[S47] C++：结构化绑定遍历
来源：http://hz.ybcxt.top/gtbgfhzasu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pycfn.com/gtjhdnnbgv.html

[S48] C++：逐行读文件
来源：http://hz.quarkkingdee.top/gtdsbrwfvf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.aizwys.cn/gtwcuxeppq.html

while (std::getline(in, line)) { }
来源：http://hz.yj202588.top/gtscrtclgu.html

[S49] C++：写文件
来源：http://hz.tian-w.cn/gtvtqarruv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.0kj1m.cn/gtxailhldx.html

[S50] C++：格式化数字
来源：http://hz.jinyuanbaomall.cn/gtgrmtbyqv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yanxiufei.cn/gtfbqjgcvz.html

[S51] C++：显式类型转换
来源：http://hz.yongpay.top/gtlocvhkco.html

static_cast<double>(a) / b
来源：http://hz.xinyue.icu/gtujgenete.html

[S52] C++：const 与 noexcept
来源：http://hz.ppjwa.cn/gtzjiqxhxy.html

int size() const noexcept { return n_; }
来源：http://hz.daxiang520.top/gtgxjtcdwl.html

[S53] C++：移动语义
来源：http://hz.chenjidiqi.icu/gtvweynfud.html

std::vector<int> w = std::move(v);
来源：http://hz.ehwqpu.com/gtfprfayuj.html

[S54] C++：异常处理
来源：http://hz.tanke756.top/gthtqibsfk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ywan-chungtsiang.top/gtihejtfdq.html

[S55] C++：结构化绑定
来源：http://hz.fengsongda.top/gtfspxpmjr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhongyouzk.top/gtikqxpdtm.html

[S56] C++：optional
来源：http://hz.52xcode.cn/gtafsrwrve.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangshuangyany.cn/gtislzekce.html

[S57] C++：编译期常量
来源：http://hz.9152youxi.cn/gtxgyxlvot.html

constexpr int N = 10;
来源：http://hz.zhoulong.xyz/gtjpylbrii.html

[S58] C++：命名空间
来源：http://hz.zhijiandao.cn/gtmdnxjpks.html


<!-- 参考信息 -->