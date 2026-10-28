代发 wailian999

[Q82] 字符长度与字节长度
来源：http://hz.jinqigfzy.top/gtrggtxfvf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yuanzhike.top/gtbjmyvcog.html

[Q83] 大小写转换
来源：http://hz.yuanzhike.top/gtgxxhugdc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cheryme.top/gttdtjpcfx.html

[Q84] 去除首尾空格
来源：http://hz.xinyue.icu/gtzvrdyscy.html

SELECT TRIM(name) FROM users;
来源：http://hz.shzxlz.cn/gtwcwarbqh.html

[Q85] 数值取整
来源：http://hz.quarkkingdee.top/gtnwattstq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangtech.top/gtjcrmbvvc.html

[Q86] 读取 JSON 字段
来源：http://hz.dashuyun.cn/gtemnsnkdn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.daxiang520.top/gtnkkhwfle.html

[Q87] JSON 字段做条件
来源：http://hz.hysaishi.cn/gtvgmclqry.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhixingplan.top/gtzmnrkbph.html

[Q88] 行转列（条件聚合）
来源：http://hz.yonumen.top/gtpasrjinf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nanxuanxn.top/gtaubfkktm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shanyushiyangtech.top/gtujkeybci.html

[Q89] 判断表是否存在
来源：http://hz.ydjk.org.cn/gtpeddvayd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.haohaochexian.top/gtthrqundk.html

[Q90] 生成序号列
来源：http://hz.yanxiufei.cn/gtqsolcgaf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yonumen.top/gtiidwknot.html

================================================================================
来源：http://hz.hammf.cn/gterotcjll.html

R. Bash 专题
来源：http://hz.jqgufenzy.top/gtdbofyrlb.html

================================================================================
来源：http://hz.yonumen.top/gtenprfxhs.html

[R01] shebang 与严格模式
来源：http://hz.316326.xyz/gtrqvvxwul.html

#!/usr/bin/env bash
来源：http://hz.snrcjt.cn/gttrxhglyo.html

set -euo pipefail
来源：http://hz.316326.xyz/gtgloezvdu.html

[R02] 变量赋值与使用
来源：http://hz.svipenyu.cn/gttnoylwlr.html

name="Tom"; echo "$name"
来源：http://hz.chenzaomai.com/gtpmzxlzhd.html

[R03] 只读变量
来源：http://hz.yvedp.cn/gtdcassoci.html

readonly PI=3.14
来源：http://hz.shanyushiyangkeji.top/gtmiryrgfo.html

[R04] 位置参数
来源：http://hz.daria6918.cn/gtbsnhdarc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnxiangtu.top/gtvmrtncwh.html

[R05] 参数默认值
来源：http://hz.zhixingplan.top/gtojkzlbhl.html

name="${1:-default}"
来源：http://hz.iojbl.cn/gtnibmqkmc.html

[R06] 判断命令是否存在
来源：http://hz.zhengqikj.top/gthrsnpqdu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.c1oappe.top/gtcoyuyxvb.html

[R07] if 判断文件
来源：http://hz.yonumen.top/gtzkembhoe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gaohongyu789.top/gtaribvnwq.html

[R08] 数值比较
来源：http://hz.yuanzhike.top/gtmpsvdkoh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.havefunace.top/gtxdzloest.html

[R09] 字符串比较
来源：http://hz.sysykeji.top/gtocityoto.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jianghu66.top/gtzhwvglcj.html

[R10] 正则匹配
来源：http://hz.haohaochexian.top/gtzqdukgrm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gaohongyu789.top/gtakwdwwxl.html

[R11] case 多分支
来源：http://hz.ehwqpu.com/gtdupujuur.html

case "$1" in
来源：http://hz.yonumen.top/gtwmfbcipi.html

start) echo "启动" ;;
来源：http://hz.xylfe.cn/gttptmoouf.html

stop)  echo "停止" ;;
来源：http://hz.pycfn.com/gtqmjquwww.html

*)     echo "未知命令" ;;
来源：http://hz.ivvv.top/gtogvsmllk.html

esac
来源：http://hz.chenlongwang.top/gtvymnstxq.html

[R12] for 遍历文件
来源：http://hz.jinyuanbaomall.cn/gtepsppqul.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yanxiufei.cn/gtopouohul.html

[R13] for 计数循环
来源：http://hz.havefunace.top/gtbdtvvkrr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhengqikj.top/gtpsdiyask.html

[R14] C 风格 for
来源：http://hz.sysykeji.top/gtszsqjiwa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xingfuxueyuan.xyz/gthkwfspfq.html

[R15] while 逐行读文件
来源：http://hz.jyoumei.cn/gtuuaipnyo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yanxiufei.cn/gtddlcmpql.html

[R16] until 等待条件
来源：http://hz.xinyue.icu/gteboieftj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yanxiufei.cn/gtdazmnlxx.html

[R17] 数组定义与取值
来源：http://hz.nwbrower.top/gtvecwfudb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yongpay.top/gtwxjwowda.html

[R18] 遍历数组
来源：http://hz.shanyushiyangkeji.top/gtfwptvglr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hnxiangtu.top/gtvdqgsoyn.html

[R19] 数组长度
来源：http://hz.jinqigufen.top/gttuovoykn.html

echo "${#arr[@]}"
来源：http://hz.jinyuanbaomall.cn/gtjrhfcosy.html

[R20] 关联数组（字典）
来源：http://hz.hnxiangtu.top/gtlxlrvgdu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gtczmpuspt.html

[R21] 字符串长度
来源：http://hz.tian-w.cn/gtljazeavu.html

echo "${#s}"
来源：http://hz.gzhubu.top/gtthfwlyyx.html

[R22] 截取子串
来源：http://hz.ywan-chungtsiang.top/gtiobcimoi.html

echo "${s:0:5}"
来源：http://hz.jiagoushi.top/gtrdafkwuq.html

[R23] 字符串替换
来源：http://hz.dianchejie.cn/gtdjhivmap.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.guannengcc.top/gtlxuiszgf.html

[R24] 大小写转换
来源：http://hz.andypj.xyz/gtkbqnsizh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258888.top/gtholmzzkw.html

[R25] 去后缀 / 去前缀
来源：http://hz.sufxvd.cn/gtwkklbrdm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuanzhike.top/gthznymhut.html

[R26] 命令替换
来源：http://hz.zhijiandao.cn/gtnwyosmur.html

now=$(date +%F); echo "$now"
来源：http://hz.zhixingplan.top/gtqebrdqxo.html

[R27] 算术展开
来源：http://hz.jinghuilouyu.cn/gtyxvoorzz.html

echo $((1 + 2 * 3))
来源：http://hz.feifeiyinyue.top/gtystlktke.html

[R28] 浮点运算
来源：http://hz.smart0.xyz/gtbjpcdien.html

echo "scale=2; 10/3" | bc
来源：http://hz.fzhhl.top/gtuelsbdln.html

[R29] 定义函数
来源：http://hz.yangfankeji.com/gtzzoyprov.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhongyouzk.top/gtsvsqweut.html

[R30] 函数返回状态码
来源：http://hz.chenzaomai.com/gtmiztvjbn.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jlsjyb.cn/gtaennrbdt.html

[R31] 局部变量
来源：http://hz.hysaishi.cn/gtjrzmgyjz.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhoulong.xyz/gtljialtio.html

[R32] 参数个数校验
来源：http://hz.yangfankeji.com/gtyasxztnj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zdqjudy.top/gtbnnvbklh.html

[R33] 捕获错误并提示行号
来源：http://hz.nwbrower.top/gthdvxnqhg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhoulong.xyz/gtriajqmwl.html

[R34] 退出时清理
来源：http://hz.yueranfly.top/gtdyxyqceu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydzc1.top/gtmlokcqqs.html

[R35] 后台执行并等待
来源：http://hz.shanyushiyangkeji.top/gttbibahqv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.snrcjt.cn/gtfbusitxa.html

[R36] 并发执行多个任务
来源：http://hz.daria6918.cn/gtlchtsizl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinqigufen.top/gtpndmvfvy.html

[R37] 把输出赋给变量
来源：http://hz.316326.xyz/gtgnllegzd.html

files=$(ls -1)
来源：http://hz.hnxiangtu.top/gthupuusxy.html

[R38] 管道串联
来源：http://hz.smart0.xyz/gtupszkncu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.birdmap.top/gtfelnloob.html

[R39] 重定向标准输出与错误
来源：http://hz.kuanghao11.cn/gtpohfqklq.html

cmd > out.log 2>&1
来源：http://hz.svipenyu.cn/gttqdtqzvv.html

[R40] 追加写日志
来源：http://hz.yuanzhike.top/gtszyjafjd.html

echo "log" >> out.log
来源：http://hz.ppjwa.cn/gtjqhqnfms.html

[R41] 丢弃输出
来源：http://hz.jinqigfzy.top/gtaxwnrgsq.html

cmd >/dev/null 2>&1
来源：http://hz.chenzaomai.com/gtochrfnxu.html

[R42] 输入重定向
来源：http://hz.smart0.xyz/gtvuocwngv.html

wc -l < a.txt
来源：http://hz.guannengcc.top/gtlbcfmwpg.html

[R43] 按名字查找文件
来源：http://hz.jqgfzy.top/gtrtxfpzcm.html

find . -name "*.log" -type f
来源：http://hz.jqgufenzy.top/gtvewapwlk.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangtech.top/gtluafmkji.html

find . -mtime -7 -type f
来源：http://hz.aizwys.cn/gtculglijt.html

[R45] 批量删除
来源：http://hz.snrcjt.cn/gtopsmwtli.html

find . -name "*.tmp" -delete
来源：http://hz.quarkkingdee.top/gtjknizvkz.html

[R46] 递归替换文件内容
来源：http://hz.chenzaomai.com/gtwaugxtxf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhaomingkeji.xyz/gtuutszazq.html

[R47] sed 单行替换
来源：http://hz.ivvv.top/gtdxbphjhv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daria6918.cn/gtaljhwacz.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gtlbwityds.html

awk '{print $1, $3}' a.txt
来源：http://hz.sweek.top/gtxnhwvxls.html

[R49] awk 带条件
来源：http://hz.cdnleiting.top/gtuluycxvi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pycfn.com/gtrsczpdol.html

[R50] awk 求和
来源：http://hz.xuetiantiany.cn/gttodzqrnh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtkqnpsyam.html

[R51] 排序去重取前几
来源：http://hz.yongpay.top/gtblmkwzpf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yonumen.top/gtsgbmqqkk.html

[R52] 统计行数
来源：http://hz.wangshuangyany.cn/gtohhorixy.html

wc -l a.txt
来源：http://hz.andypj.xyz/gtfwatchmz.html

[R53] 查看文件头与实时尾
来源：http://hz.feifeiyinyue.top/gtyerfrxrj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shzxlz.cn/gtwaglfshd.html

[R54] 比较两个文件
来源：http://hz.daria6918.cn/gtijlxglhs.html

diff a.txt b.txt
来源：http://hz.yuanzhike.top/gtgmphozjf.html

[R55] 压缩与解压
来源：http://hz.c1oappe.top/gtcwouhsyh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.pengpengdd.cyou/gtndrwxewo.html

[R56] 远程拷贝
来源：http://hz.redwolf501.top/gtegjynufb.html

scp file user@host:/path/
来源：http://hz.9152youxi.cn/gtgvdpxowe.html

[R57] 远程执行命令
来源：http://hz.zhoulong.xyz/gthwhqtpza.html

ssh user@host 'uptime'
来源：http://hz.mhx1999.top/gtlvsnhmdr.html

[R58] 下载文件
来源：http://hz.hywenlv.cn/gtznvijrcv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sxryk.cn/gtismpzmfg.html

[R59] 发 POST JSON
来源：http://hz.zhengqikj.top/gtftrwmaup.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hysaishi.cn/gtizgnpter.html

[R60] 只看 HTTP 状态码
来源：http://hz.cdnleiting.top/gtxqsrsbzc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.feifeiyinyue.top/gtmuodoqib.html

[R61] 磁盘占用
来源：http://hz.zhengqikj.top/gtsstxspeh.html

df -h;  du -sh *
来源：http://hz.nanxinkj.top/gtnazddwbg.html

[R62] 找最占空间的文件
来源：http://hz.xinyue.icu/gtdbtpfpfx.html

du -ah . | sort -rh | head -10
来源：http://hz.yvedp.cn/gtqrozdmhb.html

[R63] 内存与进程
来源：http://hz.pengpengdd.cyou/gtsxjfmzgb.html

free -h;  ps aux | grep nginx
来源：http://hz.cashguo.top/gtndikoixb.html

[R64] 结束进程
来源：http://hz.svipenyu.cn/gtrhgvtxku.html

kill -9 $(pgrep -f app.py)
来源：http://hz.9152youxi.cn/gtgdfycucb.html

[R65] 查看端口占用
来源：http://hz.sufxvd.cn/gthhjpseqk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.redwolf501.top/gtynkkjyab.html

[R66] 定时任务
来源：http://hz.nanxinkj.top/gtggxtjaja.html

crontab -e;  crontab -l
来源：http://hz.daxiang520.top/gtrqvuvqbc.html

[R67] 生成随机十六进制串
来源：http://hz.yj202588.top/gtzgrkecbc.html

openssl rand -hex 16
来源：http://hz.gaohongyu789.top/gtsubkhuhx.html

[R68] 计算文件校验值
来源：http://hz.sysykeji.top/gtdjviuwdh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gaohongyu789.top/gttceyzgik.html

[R69] 生成随机密码
来源：http://hz.guannengcc.top/gtjxqwwtqg.html

head -c 16 /dev/urandom | base64
来源：http://hz.xylfe.cn/gtidqmzwpn.html

[R70] 时间戳与互转
来源：http://hz.daria6918.cn/gtmvfrqcne.html

date +%s;  date -d @1700000000
来源：http://hz.aibaodan.cn/gtkwblqula.html

[R71] 日期格式化
来源：http://hz.zhoulong.xyz/gtfkvbfnkx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hywenlv.cn/gtcfzylwqv.html

[R72] 等待端口就绪
来源：http://hz.mhx1999.top/gtzjnftaip.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigufen.top/gtiljxfunf.html

[R73] 分割大日志
来源：http://hz.ppjwa.cn/gturfglolz.html

split -l 1000 big.log part_
来源：http://hz.zdqjudy.top/gtbekrrozm.html

[R74] 批量重命名
来源：http://hz.tanke756.top/gtguyikaif.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nanxuanxn.top/gtoiqrgrsy.html

[R75] 导出环境变量
来源：http://hz.hongshengwenyu.top/gttwyfivft.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shangyingyoupin.top/gttttcoijy.html

[R76] 使用临时文件
来源：http://hz.jqgufenzy.top/gtnwoipjoh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dashuyun.cn/gthbdooati.html

[R77] 读取用户输入
来源：http://hz.xuetiantiany.cn/gtvgvcxkah.html

read -rp "请输入: " ans
来源：http://hz.cqqwz.cn/gtmufmhrmi.html

[R78] 交互式菜单
来源：http://hz.feifeiyinyue.top/gtthakwzwd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ybcxt.top/gtunxnjyut.html

[R79] 解析命令行选项
来源：http://hz.tian-w.cn/gtmzholffa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.bjfxy.top/gtyvsxkxhr.html

[R80] 查看脚本执行耗时
来源：http://hz.9152youxi.cn/gtohqbwkgq.html

time ./run.sh
来源：http://hz.jinyuanbaomall.cn/gtgvqvuymd.html

================================================================================
来源：http://hz.tianlin.xyz/gtthydvemp.html

S. C / C++ 专题
来源：http://hz.yvedp.cn/gtolelwexr.html

================================================================================
来源：http://hz.nanxinkj.top/gtvlurbkdk.html

[S01] C：Hello World
来源：http://hz.xinyue.icu/gtdzeewgnd.html

#include <stdio.h>
来源：http://hz.shanyushiyangkeji.top/gtyheqhxqd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xziqi.cn/gtiputihdh.html

[S02] C：变量与格式化输出
来源：http://hz.yj20258888.top/gtykutktsw.html

int a = 10; printf("%d\n", a);
来源：http://hz.jqgfzy.top/gtctmdtomk.html

[S03] C：读入整数
来源：http://hz.shzxlz.cn/gtgxkuyofl.html

int x; scanf("%d", &x);
来源：http://hz.xuanzx.com/gtucyflceo.html

[S04] C：字符串复制
来源：http://hz.zhijiandao.cn/gtwarjekft.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.snrcjt.cn/gtlejxzbpa.html

[S05] C：字符串长度
来源：http://hz.shzxlz.cn/gtaemjzfgd.html

strlen(s)
来源：http://hz.316326.xyz/gtqmhszrbg.html

[S06] C：字符串比较
来源：http://hz.havefunace.top/gtvrzgewfh.html

strcmp(a, b) == 0
来源：http://hz.jinqigfzy.top/gtjevbobpr.html

[S07] C：数组遍历求和
来源：http://hz.tian-w.cn/gtkoyfoqyc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shanyushiyangkeji.top/gtuaxeorkn.html

[S08] C：动态内存分配与释放
来源：http://hz.gotoacloud.top/gtegokfdzy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenlongwang.top/gtfvunsoiu.html

[S09] C：结构体定义与初始化
来源：http://hz.52xcode.cn/gtpqmlnvzo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gogol.net.cn/gtbewfgjry.html

[S10] C：指针与解引用
来源：http://hz.meibo888.top/gthpwazisg.html

int *p = &a;  *p = 5;
来源：http://hz.zhongyouzk.top/gtlltqabig.html

[S11] C：逐行读文件
来源：http://hz.vqdsnc.cn/gtnmuirnbo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xuetiantiany.cn/gtofrgaqgm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxinkj.top/gtspxjotqj.html

fclose(f);
来源：http://hz.0kj1m.cn/gtwiffsybo.html

[S12] C：写文件
来源：http://hz.wangshuangyany.cn/gtcbzdejin.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.wangdashe.top/gtqdltwxiv.html

[S13] C：宏定义
来源：http://hz.hnxiangtu.top/gtoenezeoi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zdqjudy.top/gtvkgdnist.html

[S14] C：枚举
来源：http://hz.52xcode.cn/gtgmtpgymy.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.316326.xyz/gtlmkdjlge.html

[S15] C：类型转换
来源：http://hz.gogol.net.cn/gtfxppyahi.html

(double) a / b
来源：http://hz.snrcjt.cn/gtirveggwr.html

[S16] C：位操作置位
来源：http://hz.cashguo.top/gtjwjkbggi.html

x |= (1 << 3);
来源：http://hz.shangyingyoupin.top/gtprdovrbs.html

[S17] C：安全拼接字符串
来源：http://hz.hongshengwenyu.top/gtpsxczhgp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.birdmap.top/gtaihbhdtv.html

[S18] C：命令行参数
来源：http://hz.ydzc1.top/gtgkjcooel.html

int main(int argc, char **argv)
来源：http://hz.jinghuilouyu.cn/gtkypdgnax.html

[S19] C：快速排序
来源：http://hz.ydjk.org.cn/gtbffpwvgy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gtzbpvmoxc.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtfvjbrnec.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.bjfxy.top/gtermzatel.html

[S21] C：字符类别判断
来源：http://hz.fengsongda.top/gtmdizgpyn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cqqwz.cn/gtplribxsh.html

[S22] C：字符串转数字
来源：http://hz.svipenyu.cn/gtxkgehkyd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gzhubu.top/gtzlssovnl.html

[S23] C：随机数
来源：http://hz.cucudq.cn/gtmsgyecpb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zdqjudy.top/gtcgotrgjj.html

[S24] C：获取本地时间
来源：http://hz.jinqigfzy.top/gtryvexrqb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shzxlz.cn/gtuqburbks.html

[S25] C：内存拷贝
来源：http://hz.guowangkeji.top/gtcydpudbz.html

memcpy(dst, src, n);
来源：http://hz.yj20258.top/gtpiarcvbl.html

[S26] C：内存清零
来源：http://hz.jyoumei.cn/gtjopyfndx.html

memset(a, 0, sizeof a);
来源：http://hz.andypj.xyz/gteayoment.html

[S27] C：定义常量
来源：http://hz.yvedp.cn/gtfznznmed.html

const double PI = 3.14159;
来源：http://hz.hnqzz.top/gtfudcqxlk.html

[S28] C：静态变量
来源：http://hz.zhaomingkeji.xyz/gtjenjgjxk.html

static int counter = 0;
来源：http://hz.vqdsnc.cn/gtaqcvitvb.html

[S29] C：变参函数
来源：http://hz.yueranfly.top/gtdnnpytjy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xinyue.icu/gtkgbntpfq.html

[S30] C：头文件保护
来源：http://hz.svipenyu.cn/gtlngjwgwk.html

#ifndef X_H
来源：http://hz.0kj1m.cn/gtrwcxsxcz.html

#define X_H
来源：http://hz.hywenlv.cn/gtjxqspmqp.html

#endif
来源：http://hz.fzhhl.top/gtdjhyiyqu.html

[S31] C++：Hello World
来源：http://hz.ydjk.org.cn/gtcptbtssh.html

#include <iostream>
来源：http://hz.yuanzhike.top/gtuqdmpssc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ivvv.top/gtqtgsrrfc.html

[S32] C++：字符串
来源：http://hz.tanke756.top/gthuogqruh.html

std::string s = "hi";  s += "!";
来源：http://hz.jinqigfzy.top/gtzkezjvok.html

[S33] C++：vector 增删
来源：http://hz.ppjwa.cn/gtixzjuhgf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.daria6918.cn/gtjrbeuoee.html

[S34] C++：遍历 vector
来源：http://hz.smart0.xyz/gtzgriqthu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shzxlz.cn/gtyabndzoz.html

[S35] C++：map
来源：http://hz.aizwys.cn/gtmzzbplkp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtxlmejqsl.html

[S36] C++：unordered_map
来源：http://hz.hammf.cn/gtligabmbg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yangfankeji.com/gtubrdnfnu.html

[S37] C++：set
来源：http://hz.wangdashe.top/gtturczvfd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.pycfn.com/gtezhzhrdy.html

[S38] C++：排序
来源：http://hz.aizwys.cn/gtvgybcrrr.html

std::sort(v.begin(), v.end());
来源：http://hz.zhijiandao.cn/gtyudynxjy.html

[S39] C++：自定义比较器排序
来源：http://hz.daxiang520.top/gtddyomntj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shzxlz.cn/gtuhargegc.html

[S40] C++：查找元素
来源：http://hz.fzhhl.top/gtsimznwdh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ybcxt.top/gtrmehpbas.html

[S41] C++：类与构造函数
来源：http://hz.tianlin.xyz/gtksmwchqb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yueranfly.top/gtrvgwmosy.html

[S42] C++：继承与虚函数
来源：http://hz.vqdsnc.cn/gtvdyzxsks.html

class B : public Base { public: void f() override {} };
来源：http://hz.andypj.xyz/gtohctdayz.html

[S43] C++：智能指针
来源：http://hz.yj20258.top/gtxymwtmrm.html

auto p = std::make_unique<int>(5);
来源：http://hz.svipenyu.cn/gtyzgrpwmg.html

[S44] C++：引用传参
来源：http://hz.jinqigufen.top/gtqlzqvftu.html

void inc(int &x) { ++x; }
来源：http://hz.jinyuanbaomall.cn/gtcaqygqfq.html

[S45] C++：lambda
来源：http://hz.tanke756.top/gtzypuyqpm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sxryk.cn/gthedoaqms.html

[S46] C++：函数模板
来源：http://hz.yuanzhike.top/gtwjzbfirt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhaomingkeji.xyz/gtybltmmyd.html

[S47] C++：结构化绑定遍历
来源：http://hz.xuetiantiany.cn/gtztlsncrp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yuxming.cn/gtcguzbrqc.html

[S48] C++：逐行读文件
来源：http://hz.tanke756.top/gtjctwhwrp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.aizwys.cn/gttnwnkzyg.html

while (std::getline(in, line)) { }
来源：http://hz.hnxiangtu.top/gtzcesjyqs.html

[S49] C++：写文件
来源：http://hz.andypj.xyz/gtahfylzxc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.feifeiyinyue.top/gtctdyjlrz.html

[S50] C++：格式化数字
来源：http://hz.haohaochexian.top/gtpdxxddlg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cqqwz.cn/gttxuwvmpy.html

[S51] C++：显式类型转换
来源：http://hz.52xcode.cn/gtborktvzv.html

static_cast<double>(a) / b
来源：http://hz.yj202588.top/gtafsorhcs.html

[S52] C++：const 与 noexcept
来源：http://hz.shzxlz.cn/gtxgqtxlyl.html


<!-- 参考信息 -->