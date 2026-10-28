代发 wailian999

[Q82] 字符长度与字节长度
来源：http://hz.jiagoushi.top/gtuckgmjon.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtvupcomck.html

[Q83] 大小写转换
来源：http://hz.hammf.cn/gtgtjmhxyq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtmuszkryz.html

[Q84] 去除首尾空格
来源：http://hz.jqgufenzy.top/gtjpwedzsz.html

SELECT TRIM(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtkwzbgugh.html

[Q85] 数值取整
来源：http://hz.zhijiandao.cn/gthrzprhfg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pycfn.com/gtdnolrfev.html

[Q86] 读取 JSON 字段
来源：http://hz.aibaodan.cn/gtvhkqvofh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fzhhl.top/gtimbakzrd.html

[Q87] JSON 字段做条件
来源：http://hz.zycfv.cn/gtkfijirhy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nanxuanxn.top/gtxrveubmj.html

[Q88] 行转列（条件聚合）
来源：http://hz.ehwqpu.com/gtczslsyhg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj20258888.top/gtstymtlkg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.birdmap.top/gtfpxbnqcb.html

[Q89] 判断表是否存在
来源：http://hz.jinyuanbaomall.cn/gtdrecnsjl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tanke756.top/gtsaukhchh.html

[Q90] 生成序号列
来源：http://hz.gogol.net.cn/gtqflcwiog.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.kuanghao11.cn/gtwmoskxrc.html

================================================================================
来源：http://hz.zhijiandao.cn/gtyjlfmeja.html

R. Bash 专题
来源：http://hz.zhongyouzk.top/gtzvercipl.html

================================================================================
来源：http://hz.yangfankeji.com/gtdlnlxcgn.html

[R01] shebang 与严格模式
来源：http://hz.chenzaomai.com/gthuedsghj.html

#!/usr/bin/env bash
来源：http://hz.xingfuxueyuan.xyz/gtdatcyfpn.html

set -euo pipefail
来源：http://hz.xinyue.icu/gtepwaqejz.html

[R02] 变量赋值与使用
来源：http://hz.tianlin.xyz/gtzybcqrfh.html

name="Tom"; echo "$name"
来源：http://hz.shuidangran.top/gtgdsnettm.html

[R03] 只读变量
来源：http://hz.sxryk.cn/gtikooeifc.html

readonly PI=3.14
来源：http://hz.redwolf501.top/gtrhhdrtxu.html

[R04] 位置参数
来源：http://hz.cqqwz.cn/gtaqyhpsyt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinqigfzy.top/gtzmnazklk.html

[R05] 参数默认值
来源：http://hz.jqgufenzy.top/gthfyuatzj.html

name="${1:-default}"
来源：http://hz.pengpengdd.cyou/gtgrujnapw.html

[R06] 判断命令是否存在
来源：http://hz.smart0.xyz/gtgcknxnxu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xuanzx.com/gtbgwnvmwd.html

[R07] if 判断文件
来源：http://hz.zhongyouzk.top/gtaeeyvbsf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ehwqpu.com/gtzrdcwyce.html

[R08] 数值比较
来源：http://hz.shuidangran.top/gtbwaugbmm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yanxiufei.cn/gthkthxgnd.html

[R09] 字符串比较
来源：http://hz.jinqigfzy.top/gtxjywpuos.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydzc1.top/gtowkofloz.html

[R10] 正则匹配
来源：http://hz.sysykeji.top/gtwuufsnvc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jyoumei.cn/gtsodobpmt.html

[R11] case 多分支
来源：http://hz.hywenlv.cn/gtexfqrqfk.html

case "$1" in
来源：http://hz.andypj.xyz/gttblqkhcy.html

start) echo "启动" ;;
来源：http://hz.cucudq.cn/gtyehbojie.html

stop)  echo "停止" ;;
来源：http://hz.wangshuangyany.cn/gtizvlorxm.html

*)     echo "未知命令" ;;
来源：http://hz.jinqigufen.top/gtrqbwlnex.html

esac
来源：http://hz.aibaodan.cn/gtfrcruvgg.html

[R12] for 遍历文件
来源：http://hz.zhijiandao.cn/gtnndzfomp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yanxiufei.cn/gtofveulpa.html

[R13] for 计数循环
来源：http://hz.jqgfzy.top/gtsodwrvdg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydjk.org.cn/gtvsmtnxvw.html

[R14] C 风格 for
来源：http://hz.yueranfly.top/gtzndueshr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.aibaodan.cn/gtuiawgfju.html

[R15] while 逐行读文件
来源：http://hz.yangfankeji.com/gtegwcloyk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jyoumei.cn/gtqveudsag.html

[R16] until 等待条件
来源：http://hz.yanxiufei.cn/gtfpfvtjkz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj20258888.top/gtadhqarin.html

[R17] 数组定义与取值
来源：http://hz.tian-w.cn/gtqumbntda.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.iojbl.cn/gtcjegshio.html

[R18] 遍历数组
来源：http://hz.shangyingyoupin.top/gtqrvhqfwx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yvedp.cn/gthiydslcg.html

[R19] 数组长度
来源：http://hz.jqgfzy.top/gtrxsdzjpq.html

echo "${#arr[@]}"
来源：http://hz.iojbl.cn/gtlnakgati.html

[R20] 关联数组（字典）
来源：http://hz.tanke756.top/gtfapuxmvw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nanxuanxn.top/gtluqshshi.html

[R21] 字符串长度
来源：http://hz.nanxinkj.top/gtiombcpmw.html

echo "${#s}"
来源：http://hz.sweek.top/gtuzsiovfq.html

[R22] 截取子串
来源：http://hz.yangfankeji.com/gthulfitik.html

echo "${s:0:5}"
来源：http://hz.hongshengwenyu.top/gtygkglyyv.html

[R23] 字符串替换
来源：http://hz.zhijiandao.cn/gtnndjsflj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.fengsongda.top/gtievlhnll.html

[R24] 大小写转换
来源：http://hz.daxiang520.top/gtgfuinhbm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dianchejie.cn/gtybclmggn.html

[R25] 去后缀 / 去前缀
来源：http://hz.svipenyu.cn/gtmgqahrje.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tianlin.xyz/gthpiuyncj.html

[R26] 命令替换
来源：http://hz.cdnleiting.top/gtyllicjzw.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxinkj.top/gtcsiylrnl.html

[R27] 算术展开
来源：http://hz.zhiwuduotai.top/gtjyjhekwo.html

echo $((1 + 2 * 3))
来源：http://hz.aibaodan.cn/gtyiniumeq.html

[R28] 浮点运算
来源：http://hz.52xcode.cn/gtfncuiymx.html

echo "scale=2; 10/3" | bc
来源：http://hz.daria6918.cn/gtpotcwhoo.html

[R29] 定义函数
来源：http://hz.gzhubu.top/gtlqnucwof.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.havefunace.top/gtoxrdjspi.html

[R30] 函数返回状态码
来源：http://hz.cashguo.top/gtysaykgdc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hongshengwenyu.top/gtvbtkasxq.html

[R31] 局部变量
来源：http://hz.jianghu66.top/gteohhsinn.html

f() { local x=1; echo "$x"; }
来源：http://hz.zdqjudy.top/gticizkbfw.html

[R32] 参数个数校验
来源：http://hz.iojbl.cn/gtonehmtym.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinqigufen.top/gtgzjxuebj.html

[R33] 捕获错误并提示行号
来源：http://hz.jianghu66.top/gtuntxyrlk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.pengpengdd.cyou/gthgwbaoip.html

[R34] 退出时清理
来源：http://hz.yueranfly.top/gtxkjvkrtm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangshuangyany.cn/gtmtkbckrb.html

[R35] 后台执行并等待
来源：http://hz.yangfankeji.com/gtlglzwnoe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.feifeiyinyue.top/gtdimibxbl.html

[R36] 并发执行多个任务
来源：http://hz.yj20258888.top/gtcxzvzqdo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yuanzhike.top/gtouwjwqcu.html

[R37] 把输出赋给变量
来源：http://hz.feifeiyinyue.top/gtvhysjlkx.html

files=$(ls -1)
来源：http://hz.316326.xyz/gtrvzcmhsr.html

[R38] 管道串联
来源：http://hz.ydjk.org.cn/gtcopiddqz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhiwuduotai.top/gtifpnhgjv.html

[R39] 重定向标准输出与错误
来源：http://hz.fengsongda.top/gtditrsyvt.html

cmd > out.log 2>&1
来源：http://hz.hfpthk.cn/gtsvusawmn.html

[R40] 追加写日志
来源：http://hz.fengsongda.top/gthkqflewe.html

echo "log" >> out.log
来源：http://hz.pycfn.com/gtarmnlqnh.html

[R41] 丢弃输出
来源：http://hz.316326.xyz/gtoeinkqun.html

cmd >/dev/null 2>&1
来源：http://hz.9152youxi.cn/gtxtsbrgkw.html

[R42] 输入重定向
来源：http://hz.sufxvd.cn/gtjhvivgbe.html

wc -l < a.txt
来源：http://hz.xuanzx.com/gtoavjfaur.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtgrowmvnp.html

find . -name "*.log" -type f
来源：http://hz.chenzaomai.com/gtereebmfu.html

[R44] 按修改时间查找
来源：http://hz.cdnleiting.top/gtovuhdulx.html

find . -mtime -7 -type f
来源：http://hz.wangdashe.top/gtmdoizbti.html

[R45] 批量删除
来源：http://hz.yangfankeji.com/gtklqdmyeo.html

find . -name "*.tmp" -delete
来源：http://hz.gaohongyu789.top/gtkbcioych.html

[R46] 递归替换文件内容
来源：http://hz.ydjk.org.cn/gtwxsyexoi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daxiang520.top/gtzrvfuujw.html

[R47] sed 单行替换
来源：http://hz.zycfv.cn/gtiwggdjly.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtycodrunq.html

[R48] awk 取指定列
来源：http://hz.svipenyu.cn/gtzojhmbpp.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258.top/gtpitlppea.html

[R49] awk 带条件
来源：http://hz.yuanzhike.top/gtpudjmyqt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ydzc1.top/gtsqlahgyt.html

[R50] awk 求和
来源：http://hz.xuetiantiany.cn/gtyjorswnk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cucudq.cn/gtcxqbrvdl.html

[R51] 排序去重取前几
来源：http://hz.yueranfly.top/gtruphkaxk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cdnleiting.top/gtuzgmuhxt.html

[R52] 统计行数
来源：http://hz.ydjk.org.cn/gtdqjtilwb.html

wc -l a.txt
来源：http://hz.xingfuxueyuan.xyz/gtsxelhmcl.html

[R53] 查看文件头与实时尾
来源：http://hz.svipenyu.cn/gtgdjfsyrw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sufxvd.cn/gtujkhkufh.html

[R54] 比较两个文件
来源：http://hz.jinqigfzy.top/gtoyxtafys.html

diff a.txt b.txt
来源：http://hz.xylfe.cn/gtzlgkjqdq.html

[R55] 压缩与解压
来源：http://hz.0kj1m.cn/gtizevthot.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shanyushiyangtech.top/gtzjebrtpc.html

[R56] 远程拷贝
来源：http://hz.cheryme.top/gtyockouvy.html

scp file user@host:/path/
来源：http://hz.zhijiandao.cn/gtwakysbzf.html

[R57] 远程执行命令
来源：http://hz.shangyingyoupin.top/gtfnhbpdnm.html

ssh user@host 'uptime'
来源：http://hz.jiagoushi.top/gtzmzlhbhv.html

[R58] 下载文件
来源：http://hz.yueranfly.top/gtintbpizr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xziqi.cn/gtjjurchar.html

[R59] 发 POST JSON
来源：http://hz.dianchejie.cn/gtkmwamlpi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xuetiantiany.cn/gtdadfrniu.html

[R60] 只看 HTTP 状态码
来源：http://hz.quarkkingdee.top/gthliovpkn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.fengsongda.top/gtgerjsebp.html

[R61] 磁盘占用
来源：http://hz.andypj.xyz/gtdtnbyrsu.html

df -h;  du -sh *
来源：http://hz.tianlin.xyz/gtdqglvukx.html

[R62] 找最占空间的文件
来源：http://hz.hysaishi.cn/gtwloxxquw.html

du -ah . | sort -rh | head -10
来源：http://hz.jlsjyb.cn/gtjivuztlm.html

[R63] 内存与进程
来源：http://hz.hongshengwenyu.top/gttccfggzw.html

free -h;  ps aux | grep nginx
来源：http://hz.cdnleiting.top/gtcxzcnrjq.html

[R64] 结束进程
来源：http://hz.jqgufenzy.top/gtymqpgsrn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jqgufenzy.top/gtrttyxory.html

[R65] 查看端口占用
来源：http://hz.haohaochexian.top/gtnzesangy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guowangkeji.top/gtblhsjzbo.html

[R66] 定时任务
来源：http://hz.chenzaomai.com/gtwlztdocn.html

crontab -e;  crontab -l
来源：http://hz.jlsjyb.cn/gtbbzkcaog.html

[R67] 生成随机十六进制串
来源：http://hz.chenzaomai.com/gtrwapovgz.html

openssl rand -hex 16
来源：http://hz.yonumen.top/gtjrbyghzn.html

[R68] 计算文件校验值
来源：http://hz.cdnleiting.top/gtegzdauvj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.havefunace.top/gtlknhvibg.html

[R69] 生成随机密码
来源：http://hz.ydjk.org.cn/gthvvwmefs.html

head -c 16 /dev/urandom | base64
来源：http://hz.hysaishi.cn/gtzirqyptc.html

[R70] 时间戳与互转
来源：http://hz.ydzc1.top/gtbmnkmupc.html

date +%s;  date -d @1700000000
来源：http://hz.jqgufenzy.top/gttrexammh.html

[R71] 日期格式化
来源：http://hz.yanxiufei.cn/gtxjaawvqv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yangfankeji.com/gtearylyut.html

[R72] 等待端口就绪
来源：http://hz.pengpengdd.cyou/gtkzugygbp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xuanzx.com/gtfgvcwazn.html

[R73] 分割大日志
来源：http://hz.ywan-chungtsiang.top/gtjvemjcic.html

split -l 1000 big.log part_
来源：http://hz.chenjidiqi.icu/gtnybyucma.html

[R74] 批量重命名
来源：http://hz.sysykeji.top/gtnzghupav.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhijiandao.cn/gtmhydghed.html

[R75] 导出环境变量
来源：http://hz.jqgfzy.top/gtulannnth.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.bjfxy.top/gtcadsepaw.html

[R76] 使用临时文件
来源：http://hz.nwbrower.top/gtpcukriwu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtoqmucrvw.html

[R77] 读取用户输入
来源：http://hz.hongshengwenyu.top/gtrjpguart.html

read -rp "请输入: " ans
来源：http://hz.zhaomingkeji.xyz/gtkayiiwva.html

[R78] 交互式菜单
来源：http://hz.vqdsnc.cn/gtlodydcbr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jiagoushi.top/gtntbjhezt.html

[R79] 解析命令行选项
来源：http://hz.jinyuanbaomall.cn/gtujcrpbmp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daria6918.cn/gtgnxxodli.html

[R80] 查看脚本执行耗时
来源：http://hz.haohaochexian.top/gtfpwxxfni.html

time ./run.sh
来源：http://hz.dianchejie.cn/gtqlktzpoj.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtdyxgqokz.html

S. C / C++ 专题
来源：http://hz.sufxvd.cn/gtebctkpbx.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtmljnlexl.html

[S01] C：Hello World
来源：http://hz.gaohongyu789.top/gtjaklvjgl.html

#include <stdio.h>
来源：http://hz.jiagoushi.top/gtxvynfrol.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ydzc1.top/gtwxesyqkp.html

[S02] C：变量与格式化输出
来源：http://hz.nwbrower.top/gttguwbjfs.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxinkj.top/gtfqtxpvfi.html

[S03] C：读入整数
来源：http://hz.shangyingyoupin.top/gtreqkyodm.html

int x; scanf("%d", &x);
来源：http://hz.mhx1999.top/gtetazopjl.html

[S04] C：字符串复制
来源：http://hz.sweek.top/gtdjxcjzfp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhongyouzk.top/gtudvmkpjg.html

[S05] C：字符串长度
来源：http://hz.aibaodan.cn/gtihmkckuq.html

strlen(s)
来源：http://hz.jqgufenzy.top/gtirvekfir.html

[S06] C：字符串比较
来源：http://hz.zhoulong.xyz/gtffqgjzge.html

strcmp(a, b) == 0
来源：http://hz.jiagoushi.top/gtwergmbdv.html

[S07] C：数组遍历求和
来源：http://hz.xuetiantiany.cn/gttqadtnsq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cashguo.top/gthmdlcydj.html

[S08] C：动态内存分配与释放
来源：http://hz.shuidangran.top/gtzghzgdbd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhaomingkeji.xyz/gtqujcufrm.html

[S09] C：结构体定义与初始化
来源：http://hz.yuxming.cn/gtpwpmofdv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj202588.top/gtpqrsryir.html

[S10] C：指针与解引用
来源：http://hz.0kj1m.cn/gtqfmbqfvv.html

int *p = &a;  *p = 5;
来源：http://hz.svipenyu.cn/gtrnmfqves.html

[S11] C：逐行读文件
来源：http://hz.gogol.net.cn/gtgutsmkqx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigfzy.top/gtdilkbmkr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xylfe.cn/gtdfftcqhj.html

fclose(f);
来源：http://hz.ywan-chungtsiang.top/gtdwuqddfl.html

[S12] C：写文件
来源：http://hz.zhongyouzk.top/gtuoitdibh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yueranfly.top/gtkcbnzinz.html

[S13] C：宏定义
来源：http://hz.xylfe.cn/gttwgejhfm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xuetiantiany.cn/gtkihlepnl.html

[S14] C：枚举
来源：http://hz.zhixingplan.top/gtstvsegev.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gaohongyu789.top/gtsyyvvijr.html

[S15] C：类型转换
来源：http://hz.gotoacloud.top/gterxqmhyn.html

(double) a / b
来源：http://hz.jinyuanbaomall.cn/gthsviooio.html

[S16] C：位操作置位
来源：http://hz.daxiang520.top/gtpvswywsx.html

x |= (1 << 3);
来源：http://hz.wangshuangyany.cn/gtswgoikmv.html

[S17] C：安全拼接字符串
来源：http://hz.ehwqpu.com/gtztqgmhev.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.haohaochexian.top/gtunamfkzk.html

[S18] C：命令行参数
来源：http://hz.bjfxy.top/gtgmkhvptl.html

int main(int argc, char **argv)
来源：http://hz.feifeiyinyue.top/gtxrbozhkp.html

[S19] C：快速排序
来源：http://hz.yueranfly.top/gtmunjshuf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtynguniwh.html

[S20] C：二分查找
来源：http://hz.smart0.xyz/gtevqyqhvm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.iojbl.cn/gtfczpmqzt.html

[S21] C：字符类别判断
来源：http://hz.daria6918.cn/gtsyvgduhk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yanxiufei.cn/gtqqdxtnem.html

[S22] C：字符串转数字
来源：http://hz.ehwqpu.com/gtpkvsvcvp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydjk.org.cn/gtobuszjzm.html

[S23] C：随机数
来源：http://hz.tian-w.cn/gtnnxfnjkw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinqigufen.top/gtjrsaqrlq.html

[S24] C：获取本地时间
来源：http://hz.jqgufenzy.top/gtrtscqobs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinyuanbaomall.cn/gttxaepjgg.html

[S25] C：内存拷贝
来源：http://hz.yj20258888.top/gtdsdakuzj.html

memcpy(dst, src, n);
来源：http://hz.ybcxt.top/gtutumoulr.html

[S26] C：内存清零
来源：http://hz.yuanzhike.top/gtwcuzflzm.html

memset(a, 0, sizeof a);
来源：http://hz.cucudq.cn/gtyreuxtea.html

[S27] C：定义常量
来源：http://hz.jinqigfzy.top/gtffqcpoca.html

const double PI = 3.14159;
来源：http://hz.jiagoushi.top/gthvgqjrwu.html

[S28] C：静态变量
来源：http://hz.daxiang520.top/gtdxatfmso.html

static int counter = 0;
来源：http://hz.chenzaomai.com/gtqwnoycqd.html

[S29] C：变参函数
来源：http://hz.daxiang520.top/gtepdxprwe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenjidiqi.icu/gtshpdnoev.html

[S30] C：头文件保护
来源：http://hz.jqgufenzy.top/gtehyakovo.html

#ifndef X_H
来源：http://hz.yuxming.cn/gtbcbdrjeq.html

#define X_H
来源：http://hz.jyoumei.cn/gtltcqurbn.html

#endif
来源：http://hz.xuanzx.com/gtaikeopuc.html

[S31] C++：Hello World
来源：http://hz.ywan-chungtsiang.top/gtolfnurip.html

#include <iostream>
来源：http://hz.svipenyu.cn/gtyjwrygur.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.aizwys.cn/gtljqqanaq.html

[S32] C++：字符串
来源：http://hz.hammf.cn/gtfzorknum.html

std::string s = "hi";  s += "!";
来源：http://hz.yonumen.top/gtvkkxjbrr.html

[S33] C++：vector 增删
来源：http://hz.aizwys.cn/gtgdlvsviy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hammf.cn/gticqxdzbg.html

[S34] C++：遍历 vector
来源：http://hz.jinqigfzy.top/gtfxcmhgec.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ydjk.org.cn/gtiulxakhj.html

[S35] C++：map
来源：http://hz.c1oappe.top/gtvzzwtijv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yangfankeji.com/gtucewgvmj.html

[S36] C++：unordered_map
来源：http://hz.nwbrower.top/gtsxboyqmo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtbdwyvneh.html

[S37] C++：set
来源：http://hz.zdqjudy.top/gtnceseckl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ybcxt.top/gthncwvavm.html

[S38] C++：排序
来源：http://hz.shzxlz.cn/gtsdkyvcxe.html

std::sort(v.begin(), v.end());
来源：http://hz.hywenlv.cn/gtzgqfoikm.html

[S39] C++：自定义比较器排序
来源：http://hz.birdmap.top/gtdebnjagp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yongpay.top/gtvgvljisi.html

[S40] C++：查找元素
来源：http://hz.ehwqpu.com/gtbohbpwzs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.redwolf501.top/gtchsxlnkt.html

[S41] C++：类与构造函数
来源：http://hz.havefunace.top/gtsygutikm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.haohaochexian.top/gtbdtdsprq.html

[S42] C++：继承与虚函数
来源：http://hz.tian-w.cn/gtxolnpddw.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxuanxn.top/gtbaixarpf.html

[S43] C++：智能指针
来源：http://hz.shangyingyoupin.top/gtguosaiqg.html

auto p = std::make_unique<int>(5);
来源：http://hz.yvedp.cn/gtlipohxic.html

[S44] C++：引用传参
来源：http://hz.hongshengwenyu.top/gtepkzqsco.html

void inc(int &x) { ++x; }
来源：http://hz.pycfn.com/gthqcakbnm.html

[S45] C++：lambda
来源：http://hz.ehwqpu.com/gtswrvzgvz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xylfe.cn/gtwsiixtkd.html

[S46] C++：函数模板
来源：http://hz.guannengcc.top/gtbnsnvgwy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.snrcjt.cn/gtpwofmnmk.html

[S47] C++：结构化绑定遍历
来源：http://hz.snrcjt.cn/gttublyhmp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jlsjyb.cn/gtawfzgalt.html

[S48] C++：逐行读文件
来源：http://hz.andypj.xyz/gtswvswqdx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tianlin.xyz/gtdjqxzqpg.html

while (std::getline(in, line)) { }
来源：http://hz.xuetiantiany.cn/gtmzrhgwgs.html

[S49] C++：写文件
来源：http://hz.sxryk.cn/gtnqjdldbz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnxiangtu.top/gthyipvmjs.html

[S50] C++：格式化数字
来源：http://hz.jyoumei.cn/gthtoksqaq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigfzy.top/gtpckeaaqi.html

[S51] C++：显式类型转换
来源：http://hz.hongshengwenyu.top/gtwpbctngf.html

static_cast<double>(a) / b
来源：http://hz.jqgufenzy.top/gtejniuwsq.html

[S52] C++：const 与 noexcept
来源：http://hz.jinyuanbaomall.cn/gtkqvvveqa.html


<!-- 参考信息 -->