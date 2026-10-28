代发 wailian999

[Q82] 字符长度与字节长度
来源：http://hz.guowangkeji.top/gtlfusmilu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.smart0.xyz/gtuwgdtwin.html

[Q83] 大小写转换
来源：http://hz.zhixingplan.top/gtehisnqgs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gzhubu.top/gtwkbrszgn.html

[Q84] 去除首尾空格
来源：http://hz.hysaishi.cn/gtmnqbzqje.html

SELECT TRIM(name) FROM users;
来源：http://hz.chenzaomai.com/gtkegtrinp.html

[Q85] 数值取整
来源：http://hz.guowangkeji.top/gtgpdsgmlk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xziqi.cn/gtaugebfps.html

[Q86] 读取 JSON 字段
来源：http://hz.jinyuanbaomall.cn/gtetupkonc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yueranfly.top/gtakerjqsi.html

[Q87] JSON 字段做条件
来源：http://hz.xuetiantiany.cn/gtljfnooda.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.fengsongda.top/gtjgduqmba.html

[Q88] 行转列（条件聚合）
来源：http://hz.vqdsnc.cn/gtfyeamxzi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yongpay.top/gtptddweyp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinqigufen.top/gtdasitjts.html

[Q89] 判断表是否存在
来源：http://hz.yonumen.top/gtckemshuq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xinyue.icu/gtfgpmjrwv.html

[Q90] 生成序号列
来源：http://hz.cashguo.top/gtzvhxmdrx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nanxuanxn.top/gtypuyluis.html

================================================================================
来源：http://hz.xuanzx.com/gtllgnkvjk.html

R. Bash 专题
来源：http://hz.tian-w.cn/gtxvpdeydo.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtwlzbcpgm.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangtech.top/gtcjzkrcxx.html

#!/usr/bin/env bash
来源：http://hz.gogol.net.cn/gtrhevvhte.html

set -euo pipefail
来源：http://hz.xuetiantiany.cn/gtnaarybqj.html

[R02] 变量赋值与使用
来源：http://hz.haohaochexian.top/gtqkfxycku.html

name="Tom"; echo "$name"
来源：http://hz.dianchejie.cn/gtwjzguxpp.html

[R03] 只读变量
来源：http://hz.yj202588.top/gtbxqbcapb.html

readonly PI=3.14
来源：http://hz.zhongyouzk.top/gtnurjdyzq.html

[R04] 位置参数
来源：http://hz.sysykeji.top/gttxlyvbwa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yanxiufei.cn/gtvqoqqfxe.html

[R05] 参数默认值
来源：http://hz.wangdashe.top/gtcgkqvmzb.html

name="${1:-default}"
来源：http://hz.jiagoushi.top/gtsbalgteq.html

[R06] 判断命令是否存在
来源：http://hz.bjfxy.top/gthfeuozwg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zycfv.cn/gtiwnfxkjr.html

[R07] if 判断文件
来源：http://hz.sufxvd.cn/gtexxkbfzo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yanxiufei.cn/gtqhyjimro.html

[R08] 数值比较
来源：http://hz.wangdashe.top/gtagohlbaf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zdqjudy.top/gtuspxkapr.html

[R09] 字符串比较
来源：http://hz.meibo888.top/gthcgjjngj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuetiantiany.cn/gtjnejpygx.html

[R10] 正则匹配
来源：http://hz.pengpengdd.cyou/gthvvchcpv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shuidangran.top/gtcpsefhbl.html

[R11] case 多分支
来源：http://hz.jinqigfzy.top/gtgnjrhmgz.html

case "$1" in
来源：http://hz.jinghuilouyu.cn/gtlyffyuiu.html

start) echo "启动" ;;
来源：http://hz.wangshuangyany.cn/gtuqpqxbnl.html

stop)  echo "停止" ;;
来源：http://hz.xziqi.cn/gtnmxfsose.html

*)     echo "未知命令" ;;
来源：http://hz.zhaomingkeji.xyz/gtmgnihtpi.html

esac
来源：http://hz.chenjidiqi.icu/gtnbcvnzub.html

[R12] for 遍历文件
来源：http://hz.nanxuanxn.top/gtfxcwsbol.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guannengcc.top/gtauuuyxzt.html

[R13] for 计数循环
来源：http://hz.jinghuilouyu.cn/gtjidsdvjo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.snrcjt.cn/gtnvesqnaz.html

[R14] C 风格 for
来源：http://hz.hnqzz.top/gttglonsjz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.pycfn.com/gttqenmklw.html

[R15] while 逐行读文件
来源：http://hz.ivvv.top/gtwlawmztx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guowangkeji.top/gtwfrizwvu.html

[R16] until 等待条件
来源：http://hz.fengsongda.top/gtotpdjyku.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.0kj1m.cn/gtnckgpjpu.html

[R17] 数组定义与取值
来源：http://hz.sweek.top/gtshwhlndw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.pengpengdd.cyou/gtqutkcjxd.html

[R18] 遍历数组
来源：http://hz.chenzaomai.com/gtigrgrtxr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sxryk.cn/gtlrfnsdvk.html

[R19] 数组长度
来源：http://hz.yuanzhike.top/gtjbhwoilz.html

echo "${#arr[@]}"
来源：http://hz.0kj1m.cn/gtmmtocaay.html

[R20] 关联数组（字典）
来源：http://hz.bjfxy.top/gtuztotakg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gzhubu.top/gtubjpicud.html

[R21] 字符串长度
来源：http://hz.cucudq.cn/gtvfxeqwzg.html

echo "${#s}"
来源：http://hz.cucudq.cn/gtvpboaahf.html

[R22] 截取子串
来源：http://hz.feifeiyinyue.top/gtjsutbosh.html

echo "${s:0:5}"
来源：http://hz.jinyuanbaomall.cn/gthqikeobi.html

[R23] 字符串替换
来源：http://hz.yvedp.cn/gtvkhbdgmv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xinyue.icu/gtjhwbabzp.html

[R24] 大小写转换
来源：http://hz.hammf.cn/gtrhzvtadg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jlsjyb.cn/gtqhhrtzdj.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenjidiqi.icu/gtumvglyig.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhixingplan.top/gticrqnicp.html

[R26] 命令替换
来源：http://hz.c1oappe.top/gtceasrbaw.html

now=$(date +%F); echo "$now"
来源：http://hz.shanyushiyangtech.top/gttpgrdidh.html

[R27] 算术展开
来源：http://hz.hammf.cn/gtajouzwmi.html

echo $((1 + 2 * 3))
来源：http://hz.chenjidiqi.icu/gtulrqbcrh.html

[R28] 浮点运算
来源：http://hz.xuanzx.com/gtrykvtmja.html

echo "scale=2; 10/3" | bc
来源：http://hz.dianchejie.cn/gtnipekbxb.html

[R29] 定义函数
来源：http://hz.daria6918.cn/gtnzibhbxk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgfzy.top/gtaagsrcac.html

[R30] 函数返回状态码
来源：http://hz.snrcjt.cn/gtmnzsriyv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yanxiufei.cn/gtecorayun.html

[R31] 局部变量
来源：http://hz.shzxlz.cn/gtcpplmqir.html

f() { local x=1; echo "$x"; }
来源：http://hz.shuidangran.top/gtshtzaiun.html

[R32] 参数个数校验
来源：http://hz.shangyingyoupin.top/gtxsaapatq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.birdmap.top/gtiqvflvsg.html

[R33] 捕获错误并提示行号
来源：http://hz.ehwqpu.com/gtknipaewx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj202588.top/gtvguzzrbc.html

[R34] 退出时清理
来源：http://hz.gogol.net.cn/gtxnnjptsi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtfrzohvnm.html

[R35] 后台执行并等待
来源：http://hz.zhixingplan.top/gturcjxhdd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.pengpengdd.cyou/gtllpfjrqe.html

[R36] 并发执行多个任务
来源：http://hz.feifeiyinyue.top/gtefbtsnvb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sysykeji.top/gttfwauphp.html

[R37] 把输出赋给变量
来源：http://hz.snrcjt.cn/gttjiiwofs.html

files=$(ls -1)
来源：http://hz.ydjk.org.cn/gtgwgyxrzq.html

[R38] 管道串联
来源：http://hz.c1oappe.top/gtxxmawplh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hongshengwenyu.top/gtpiodcqyk.html

[R39] 重定向标准输出与错误
来源：http://hz.52xcode.cn/gtmfquigsa.html

cmd > out.log 2>&1
来源：http://hz.zhaomingkeji.xyz/gtmpdjmpxy.html

[R40] 追加写日志
来源：http://hz.quarkkingdee.top/gtkfgahsvr.html

echo "log" >> out.log
来源：http://hz.svipenyu.cn/gtuhbqiyaf.html

[R41] 丢弃输出
来源：http://hz.jinghuilouyu.cn/gtpxpiqumv.html

cmd >/dev/null 2>&1
来源：http://hz.cdnleiting.top/gtquljgrxw.html

[R42] 输入重定向
来源：http://hz.zycfv.cn/gtaolkjcmq.html

wc -l < a.txt
来源：http://hz.jlsjyb.cn/gtcwkuxfzy.html

[R43] 按名字查找文件
来源：http://hz.yanxiufei.cn/gttvfmnwpl.html

find . -name "*.log" -type f
来源：http://hz.sysykeji.top/gtyaayqxfs.html

[R44] 按修改时间查找
来源：http://hz.haohaochexian.top/gtujvebong.html

find . -mtime -7 -type f
来源：http://hz.birdmap.top/gtnrtszljg.html

[R45] 批量删除
来源：http://hz.xuetiantiany.cn/gtcnkginsg.html

find . -name "*.tmp" -delete
来源：http://hz.jyoumei.cn/gtnwrdjwnh.html

[R46] 递归替换文件内容
来源：http://hz.sweek.top/gtpuljvyds.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.bjfxy.top/gtcbnykfmm.html

[R47] sed 单行替换
来源：http://hz.cdnleiting.top/gtzfqqixoe.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258.top/gtxajwjcbn.html

[R48] awk 取指定列
来源：http://hz.yongpay.top/gtiitzyqnd.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhengqikj.top/gtlfmsanjk.html

[R49] awk 带条件
来源：http://hz.ywan-chungtsiang.top/gtoccuydxx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zdqjudy.top/gtrubzjvbg.html

[R50] awk 求和
来源：http://hz.xziqi.cn/gtjieguvcz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guowangkeji.top/gthdpkeomx.html

[R51] 排序去重取前几
来源：http://hz.zhixingplan.top/gtujjthywo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cheryme.top/gtqaouotvd.html

[R52] 统计行数
来源：http://hz.zdqjudy.top/gtvlqugqbo.html

wc -l a.txt
来源：http://hz.yonumen.top/gtjnvljtmm.html

[R53] 查看文件头与实时尾
来源：http://hz.pycfn.com/gtvzvykush.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.haohaochexian.top/gtvmwezqjo.html

[R54] 比较两个文件
来源：http://hz.gaohongyu789.top/gtghfhwveh.html

diff a.txt b.txt
来源：http://hz.chenlongwang.top/gtmoczpgpp.html

[R55] 压缩与解压
来源：http://hz.haohaochexian.top/gtslrvqkqt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigufen.top/gtdhynufsy.html

[R56] 远程拷贝
来源：http://hz.yongpay.top/gtrwctrsgb.html

scp file user@host:/path/
来源：http://hz.andypj.xyz/gtuhqjzxre.html

[R57] 远程执行命令
来源：http://hz.meibo888.top/gtyktmzsie.html

ssh user@host 'uptime'
来源：http://hz.c1oappe.top/gtbqprnwhw.html

[R58] 下载文件
来源：http://hz.shanyushiyangtech.top/gtonchyvzo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.kuanghao11.cn/gtikyzyppm.html

[R59] 发 POST JSON
来源：http://hz.jiagoushi.top/gtrxazhkpy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydzc1.top/gtzralxecn.html

[R60] 只看 HTTP 状态码
来源：http://hz.pycfn.com/gtwgcwwgjl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinyuanbaomall.cn/gtepwqezhy.html

[R61] 磁盘占用
来源：http://hz.hnxiangtu.top/gtyuotmbuy.html

df -h;  du -sh *
来源：http://hz.yuanzhike.top/gtlbvuhqeb.html

[R62] 找最占空间的文件
来源：http://hz.jinqigfzy.top/gtepaopcyj.html

du -ah . | sort -rh | head -10
来源：http://hz.sxryk.cn/gtmskrfbky.html

[R63] 内存与进程
来源：http://hz.fzhhl.top/gtiwibxwul.html

free -h;  ps aux | grep nginx
来源：http://hz.tianlin.xyz/gttyaxydtn.html

[R64] 结束进程
来源：http://hz.sysykeji.top/gtrjfdfgtv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenzaomai.com/gtherpsmro.html

[R65] 查看端口占用
来源：http://hz.yuanzhike.top/gtmtnsyvvy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhengqikj.top/gtihkvyqhm.html

[R66] 定时任务
来源：http://hz.ppjwa.cn/gtaelijfxu.html

crontab -e;  crontab -l
来源：http://hz.svipenyu.cn/gthuidyrft.html

[R67] 生成随机十六进制串
来源：http://hz.shanyushiyangtech.top/gtbebqchqz.html

openssl rand -hex 16
来源：http://hz.xinyue.icu/gtqmwvrpad.html

[R68] 计算文件校验值
来源：http://hz.xylfe.cn/gtymekjrux.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ehwqpu.com/gtkzbqxbud.html

[R69] 生成随机密码
来源：http://hz.hnqzz.top/gtguavplwj.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhiwuduotai.top/gtuvphpddj.html

[R70] 时间戳与互转
来源：http://hz.jlsjyb.cn/gtgnuzuhbm.html

date +%s;  date -d @1700000000
来源：http://hz.316326.xyz/gtaqsvilpa.html

[R71] 日期格式化
来源：http://hz.cdnleiting.top/gtbfkhdmwq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zycfv.cn/gtstuzfkji.html

[R72] 等待端口就绪
来源：http://hz.gzhubu.top/gthnqsqfpl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.iojbl.cn/gtwbkgvqxi.html

[R73] 分割大日志
来源：http://hz.jqgufenzy.top/gtzxycatnr.html

split -l 1000 big.log part_
来源：http://hz.svipenyu.cn/gtlblwfcup.html

[R74] 批量重命名
来源：http://hz.sufxvd.cn/gtgkedlkfa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ivvv.top/gttvvfwhwt.html

[R75] 导出环境变量
来源：http://hz.yangfankeji.com/gtkukaxrpf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenlongwang.top/gtauzmhzum.html

[R76] 使用临时文件
来源：http://hz.meibo888.top/gtdvzoheua.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhengqikj.top/gtsaddazqv.html

[R77] 读取用户输入
来源：http://hz.snrcjt.cn/gtnlyioeuf.html

read -rp "请输入: " ans
来源：http://hz.cucudq.cn/gtjjvnfdol.html

[R78] 交互式菜单
来源：http://hz.cqqwz.cn/gtlhskjfsx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nanxinkj.top/gtagdlhyog.html

[R79] 解析命令行选项
来源：http://hz.yj20258888.top/gtjdsoybpq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.redwolf501.top/gtzeslfeok.html

[R80] 查看脚本执行耗时
来源：http://hz.snrcjt.cn/gtcljsvacx.html

time ./run.sh
来源：http://hz.zhijiandao.cn/gtqvzyjfml.html

================================================================================
来源：http://hz.jianghu66.top/gtdbpvrylo.html

S. C / C++ 专题
来源：http://hz.cqqwz.cn/gtnpnmqwdv.html

================================================================================
来源：http://hz.pycfn.com/gtkehesjfm.html

[S01] C：Hello World
来源：http://hz.nanxuanxn.top/gtjkuzofgb.html

#include <stdio.h>
来源：http://hz.jianghu66.top/gtfmdgyvwn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zdqjudy.top/gtythcusob.html

[S02] C：变量与格式化输出
来源：http://hz.zhaomingkeji.xyz/gtcpcgwgit.html

int a = 10; printf("%d\n", a);
来源：http://hz.ehwqpu.com/gttywfwcfa.html

[S03] C：读入整数
来源：http://hz.fengsongda.top/gtmemepxnn.html

int x; scanf("%d", &x);
来源：http://hz.shzxlz.cn/gtsbaebjfl.html

[S04] C：字符串复制
来源：http://hz.xinyue.icu/gtbwfwxuvd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yongpay.top/gtfvflgzfa.html

[S05] C：字符串长度
来源：http://hz.sufxvd.cn/gtvffapbxq.html

strlen(s)
来源：http://hz.aizwys.cn/gtzstcpoft.html

[S06] C：字符串比较
来源：http://hz.ywan-chungtsiang.top/gtptqdlmjd.html

strcmp(a, b) == 0
来源：http://hz.nwbrower.top/gtddyfcnlx.html

[S07] C：数组遍历求和
来源：http://hz.xuetiantiany.cn/gtjajgxexd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhijiandao.cn/gtduyndljj.html

[S08] C：动态内存分配与释放
来源：http://hz.dashuyun.cn/gtbalpttkm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cdnleiting.top/gtnktyvhvz.html

[S09] C：结构体定义与初始化
来源：http://hz.xingfuxueyuan.xyz/gtfituccgx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shanyushiyangtech.top/gtnnouffgk.html

[S10] C：指针与解引用
来源：http://hz.ppjwa.cn/gtfvitcxil.html

int *p = &a;  *p = 5;
来源：http://hz.jinqigfzy.top/gtgfjskdoj.html

[S11] C：逐行读文件
来源：http://hz.yueranfly.top/gtpkftifyv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yuanzhike.top/gtdeqpbvvn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenzaomai.com/gtfurxwnzk.html

fclose(f);
来源：http://hz.yuanzhike.top/gtxusafkhp.html

[S12] C：写文件
来源：http://hz.gzhubu.top/gtledgspoe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zdqjudy.top/gtbmleikpa.html

[S13] C：宏定义
来源：http://hz.dashuyun.cn/gtdqqxcpma.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinghuilouyu.cn/gtwdsjmnhq.html

[S14] C：枚举
来源：http://hz.hammf.cn/gtqrmbpkyr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yueranfly.top/gtwuzscsbd.html

[S15] C：类型转换
来源：http://hz.chenzaomai.com/gtfwcyzmee.html

(double) a / b
来源：http://hz.jiagoushi.top/gtjucqhvjk.html

[S16] C：位操作置位
来源：http://hz.yj202588.top/gtoznirtfx.html

x |= (1 << 3);
来源：http://hz.birdmap.top/gtfchwxdjs.html

[S17] C：安全拼接字符串
来源：http://hz.fzhhl.top/gtysjeirla.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgfzy.top/gtxclrpuuo.html

[S18] C：命令行参数
来源：http://hz.hnqzz.top/gtgkvshgih.html

int main(int argc, char **argv)
来源：http://hz.chenlongwang.top/gtkqpqxiux.html

[S19] C：快速排序
来源：http://hz.gogol.net.cn/gtrkhcxgsx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtmcuezsdi.html

[S20] C：二分查找
来源：http://hz.fengsongda.top/gtgxtjhnov.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtyhcjjzyw.html

[S21] C：字符类别判断
来源：http://hz.yuanzhike.top/gtnvkxdijn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guannengcc.top/gtbrspmnzy.html

[S22] C：字符串转数字
来源：http://hz.fzhhl.top/gtnhonlkqs.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.wangshuangyany.cn/gttbwuigez.html

[S23] C：随机数
来源：http://hz.guowangkeji.top/gtibfhxoal.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinyuanbaomall.cn/gtxyopsbro.html

[S24] C：获取本地时间
来源：http://hz.jinqigfzy.top/gtngphkbyi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhongyouzk.top/gtllixflsy.html

[S25] C：内存拷贝
来源：http://hz.gogol.net.cn/gtxtlhosoe.html

memcpy(dst, src, n);
来源：http://hz.yvedp.cn/gtrewkjgov.html

[S26] C：内存清零
来源：http://hz.zhijiandao.cn/gtjfgozlbi.html

memset(a, 0, sizeof a);
来源：http://hz.yj20258.top/gtpauffdcr.html

[S27] C：定义常量
来源：http://hz.cdnleiting.top/gtvkkjjuip.html

const double PI = 3.14159;
来源：http://hz.quarkkingdee.top/gtvcimbdcu.html

[S28] C：静态变量
来源：http://hz.gotoacloud.top/gtiklkpazd.html

static int counter = 0;
来源：http://hz.nwbrower.top/gtjjaqjgrs.html

[S29] C：变参函数
来源：http://hz.yuxming.cn/gtuefkibcn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tianlin.xyz/gtjnziufha.html

[S30] C：头文件保护
来源：http://hz.chenzaomai.com/gtpgpuxxlk.html

#ifndef X_H
来源：http://hz.yj20258.top/gtanbmngey.html

#define X_H
来源：http://hz.yueranfly.top/gtybfwhstt.html

#endif
来源：http://hz.yj20258888.top/gtrciwahoy.html

[S31] C++：Hello World
来源：http://hz.quarkkingdee.top/gtoycubsaa.html

#include <iostream>
来源：http://hz.fzhhl.top/gtlbudzzrr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hammf.cn/gthqfmodse.html

[S32] C++：字符串
来源：http://hz.ppjwa.cn/gtsqujvemu.html

std::string s = "hi";  s += "!";
来源：http://hz.yuanzhike.top/gtsnvpkzwm.html

[S33] C++：vector 增删
来源：http://hz.vqdsnc.cn/gtfpzalqto.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gaohongyu789.top/gtcwwvkzgn.html

[S34] C++：遍历 vector
来源：http://hz.aibaodan.cn/gtjtpdmlft.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.0kj1m.cn/gtivsjqrdq.html

[S35] C++：map
来源：http://hz.iojbl.cn/gtjaldxfau.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtahxewxnt.html

[S36] C++：unordered_map
来源：http://hz.kuanghao11.cn/gtgzcagigo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtwaakuqff.html

[S37] C++：set
来源：http://hz.nanxuanxn.top/gtidfwnhoe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.svipenyu.cn/gtgbwqektg.html

[S38] C++：排序
来源：http://hz.hfpthk.cn/gtcfzxqzeo.html

std::sort(v.begin(), v.end());
来源：http://hz.316326.xyz/gtvqqecezl.html

[S39] C++：自定义比较器排序
来源：http://hz.shanyushiyangkeji.top/gtngoxrxgj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dashuyun.cn/gtqysuaets.html

[S40] C++：查找元素
来源：http://hz.cqqwz.cn/gthebpzfbo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxinkj.top/gtmzsgcqkf.html

[S41] C++：类与构造函数
来源：http://hz.gotoacloud.top/gtwtrnddto.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinyuanbaomall.cn/gtwlgkxsuf.html

[S42] C++：继承与虚函数
来源：http://hz.zdqjudy.top/gtutkayqye.html

class B : public Base { public: void f() override {} };
来源：http://hz.dianchejie.cn/gtbiamiwil.html

[S43] C++：智能指针
来源：http://hz.andypj.xyz/gtjzxrdbzg.html

auto p = std::make_unique<int>(5);
来源：http://hz.cdnleiting.top/gtcfkjulib.html

[S44] C++：引用传参
来源：http://hz.zhaomingkeji.xyz/gtmwezhool.html

void inc(int &x) { ++x; }
来源：http://hz.andypj.xyz/gtjsiydjhq.html

[S45] C++：lambda
来源：http://hz.aibaodan.cn/gtlbzfudwe.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ivvv.top/gtybffbsqp.html

[S46] C++：函数模板
来源：http://hz.nanxinkj.top/gtfchvkiqv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.c1oappe.top/gtkzpmfmtm.html

[S47] C++：结构化绑定遍历
来源：http://hz.aibaodan.cn/gtbqqdrkuj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pengpengdd.cyou/gtxedvaoim.html

[S48] C++：逐行读文件
来源：http://hz.hammf.cn/gttldjmboz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hfpthk.cn/gtmvvabnzn.html

while (std::getline(in, line)) { }
来源：http://hz.dashuyun.cn/gtqsfuvdga.html

[S49] C++：写文件
来源：http://hz.xuetiantiany.cn/gtpnqbqcbx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.havefunace.top/gttsoekmzz.html

[S50] C++：格式化数字
来源：http://hz.hongshengwenyu.top/gtkduprvga.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ydzc1.top/gtvngrwkuy.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangkeji.top/gtnksxozvj.html

static_cast<double>(a) / b
来源：http://hz.zycfv.cn/gtmdsvuysh.html

[S52] C++：const 与 noexcept
来源：http://hz.kuanghao11.cn/gtukiwxivo.html


<!-- 参考信息 -->