代发 wailian999

[Q76] 按天统计
来源：http://hz.haohaochexian.top/gtvmhjnlwz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shzxlz.cn/gtyillkcdy.html

[Q77] 时间加减
来源：http://hz.hywenlv.cn/gtehzluhpk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gtmwmuvwkj.html

[Q78] 当前时间
来源：http://hz.andypj.xyz/gtlyktyawi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinyuanbaomall.cn/gtcaybwmmm.html

[Q79] 字符串拼接
来源：http://hz.jianghu66.top/gttqbutmji.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xylfe.cn/gtiwwyupqy.html

[Q80] 字符串截取
来源：http://hz.gaohongyu789.top/gttxniualx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sysykeji.top/gtvbucnqvf.html

[Q81] 字符串替换
来源：http://hz.bjfxy.top/gtjzckjyyb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xinyue.icu/gttrxnpjgm.html

[Q82] 字符长度与字节长度
来源：http://hz.chenjidiqi.icu/gtltmdsodl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jlsjyb.cn/gtttuagjny.html

[Q83] 大小写转换
来源：http://hz.feifeiyinyue.top/gtcqtcckvt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yonumen.top/gtgobtmbkd.html

[Q84] 去除首尾空格
来源：http://hz.yongpay.top/gticzimrgx.html

SELECT TRIM(name) FROM users;
来源：http://hz.hysaishi.cn/gtsisryhdb.html

[Q85] 数值取整
来源：http://hz.ydzc1.top/gtssonbxuh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nwbrower.top/gtxqantpjp.html

[Q86] 读取 JSON 字段
来源：http://hz.birdmap.top/gtqraminym.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sweek.top/gtbqjegona.html

[Q87] JSON 字段做条件
来源：http://hz.ydzc1.top/gtyptjetqb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ehwqpu.com/gtwtwujhxo.html

[Q88] 行转列（条件聚合）
来源：http://hz.52xcode.cn/gtnrmblsdo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.fengsongda.top/gtaosgqcgr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtzbmcqbyg.html

[Q89] 判断表是否存在
来源：http://hz.kuanghao11.cn/gtibjdxhdf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.birdmap.top/gtnzbhkvvy.html

[Q90] 生成序号列
来源：http://hz.yuanzhike.top/gtgfjkvzei.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xuetiantiany.cn/gtzjkjbdph.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtfqpuliez.html

R. Bash 专题
来源：http://hz.yj20258.top/gthqjdmyel.html

================================================================================
来源：http://hz.aizwys.cn/gtbidfdvic.html

[R01] shebang 与严格模式
来源：http://hz.nanxinkj.top/gtoznbxfei.html

#!/usr/bin/env bash
来源：http://hz.jqgufenzy.top/gtzifgvyxf.html

set -euo pipefail
来源：http://hz.jinyuanbaomall.cn/gtbtkzcagv.html

[R02] 变量赋值与使用
来源：http://hz.bjfxy.top/gtdqwndbpk.html

name="Tom"; echo "$name"
来源：http://hz.sxryk.cn/gtvuuucupv.html

[R03] 只读变量
来源：http://hz.ybcxt.top/gtqnjiqpdg.html

readonly PI=3.14
来源：http://hz.dianchejie.cn/gtcuxnyegm.html

[R04] 位置参数
来源：http://hz.xuetiantiany.cn/gtjtshbnyo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.dianchejie.cn/gtoeidqcys.html

[R05] 参数默认值
来源：http://hz.tanke756.top/gteqamfqiz.html

name="${1:-default}"
来源：http://hz.nwbrower.top/gtdijndicv.html

[R06] 判断命令是否存在
来源：http://hz.jinyuanbaomall.cn/gtnrsupzqo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xziqi.cn/gtziwspvau.html

[R07] if 判断文件
来源：http://hz.zycfv.cn/gtlyvnzfqm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.havefunace.top/gtrovidafw.html

[R08] 数值比较
来源：http://hz.hammf.cn/gtmulpwpex.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tanke756.top/gtxeothido.html

[R09] 字符串比较
来源：http://hz.yj20258888.top/gtkqrltrks.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xziqi.cn/gtgrvipfkt.html

[R10] 正则匹配
来源：http://hz.redwolf501.top/gtcimcjgca.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xziqi.cn/gtpsjatmhr.html

[R11] case 多分支
来源：http://hz.xinyue.icu/gtldvcwwno.html

case "$1" in
来源：http://hz.ybcxt.top/gtgmavvcin.html

start) echo "启动" ;;
来源：http://hz.pycfn.com/gtqtdukykq.html

stop)  echo "停止" ;;
来源：http://hz.bjfxy.top/gtshyrfjkc.html

*)     echo "未知命令" ;;
来源：http://hz.andypj.xyz/gtppecbxqz.html

esac
来源：http://hz.yj20258.top/gtzvsulumz.html

[R12] for 遍历文件
来源：http://hz.jyoumei.cn/gtywgvpzfa.html

for f in *.txt; do echo "$f"; done
来源：http://hz.pycfn.com/gtknsovryi.html

[R13] for 计数循环
来源：http://hz.cheryme.top/gtmyepgzgf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtdycoiloo.html

[R14] C 风格 for
来源：http://hz.feifeiyinyue.top/gtlmkitkpy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.9152youxi.cn/gtsmveigrc.html

[R15] while 逐行读文件
来源：http://hz.hnqzz.top/gtopxaujph.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenlongwang.top/gtsmcqsogc.html

[R16] until 等待条件
来源：http://hz.svipenyu.cn/gtqkmlirqw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.wangdashe.top/gtceuabfar.html

[R17] 数组定义与取值
来源：http://hz.hammf.cn/gtzclrqqab.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shanyushiyangkeji.top/gtvhvqocjm.html

[R18] 遍历数组
来源：http://hz.tianlin.xyz/gtsynfazhk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cheryme.top/gtzvjwryvs.html

[R19] 数组长度
来源：http://hz.shuidangran.top/gtclzsvofn.html

echo "${#arr[@]}"
来源：http://hz.yj20258.top/gtarbeiopf.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtuwbxpqbk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinqigfzy.top/gtoqrsyddl.html

[R21] 字符串长度
来源：http://hz.yuxming.cn/gtmjtvoypz.html

echo "${#s}"
来源：http://hz.quarkkingdee.top/gtodbspfkp.html

[R22] 截取子串
来源：http://hz.hysaishi.cn/gtuiceifag.html

echo "${s:0:5}"
来源：http://hz.redwolf501.top/gtsjowkuga.html

[R23] 字符串替换
来源：http://hz.hnxiangtu.top/gtxbatbmmq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.guannengcc.top/gtblmpdxvr.html

[R24] 大小写转换
来源：http://hz.bjfxy.top/gtthqtlcif.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daxiang520.top/gtthwhbkyv.html

[R25] 去后缀 / 去前缀
来源：http://hz.kuanghao11.cn/gtkbkqoxkk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cdnleiting.top/gtndpzlnjp.html

[R26] 命令替换
来源：http://hz.shanyushiyangkeji.top/gtbclotppn.html

now=$(date +%F); echo "$now"
来源：http://hz.zhijiandao.cn/gtolctogud.html

[R27] 算术展开
来源：http://hz.xylfe.cn/gteexdenbc.html

echo $((1 + 2 * 3))
来源：http://hz.jyoumei.cn/gtoldtrewl.html

[R28] 浮点运算
来源：http://hz.ehwqpu.com/gtcqhkupfd.html

echo "scale=2; 10/3" | bc
来源：http://hz.mhx1999.top/gtlbkrwxzv.html

[R29] 定义函数
来源：http://hz.pycfn.com/gtittfvicm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yongpay.top/gteblebheo.html

[R30] 函数返回状态码
来源：http://hz.aibaodan.cn/gtcnvexfxq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cqqwz.cn/gthtbnxkwt.html

[R31] 局部变量
来源：http://hz.feifeiyinyue.top/gtvermomyo.html

f() { local x=1; echo "$x"; }
来源：http://hz.bjfxy.top/gtmghtedzn.html

[R32] 参数个数校验
来源：http://hz.xziqi.cn/gtskxtpxfl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shanyushiyangtech.top/gtbwklljul.html

[R33] 捕获错误并提示行号
来源：http://hz.jiagoushi.top/gtwtpqevgg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ydzc1.top/gteptnjudh.html

[R34] 退出时清理
来源：http://hz.hywenlv.cn/gtpmncrpgr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gthamqvnpv.html

[R35] 后台执行并等待
来源：http://hz.quarkkingdee.top/gtpxprfkdl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.quarkkingdee.top/gtulukhtnr.html

[R36] 并发执行多个任务
来源：http://hz.yuxming.cn/gtksiwhsop.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jqgfzy.top/gtuafixcdt.html

[R37] 把输出赋给变量
来源：http://hz.hnxiangtu.top/gtfqsewvrq.html

files=$(ls -1)
来源：http://hz.gotoacloud.top/gtkdannqsy.html

[R38] 管道串联
来源：http://hz.sysykeji.top/gtahzrbicb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ivvv.top/gtrzurbjfz.html

[R39] 重定向标准输出与错误
来源：http://hz.zhoulong.xyz/gtwuwpqixh.html

cmd > out.log 2>&1
来源：http://hz.feifeiyinyue.top/gtsrujdpvv.html

[R40] 追加写日志
来源：http://hz.redwolf501.top/gtzgdxhiva.html

echo "log" >> out.log
来源：http://hz.zhaomingkeji.xyz/gtbeizwrqm.html

[R41] 丢弃输出
来源：http://hz.jinyuanbaomall.cn/gtccjlmmgn.html

cmd >/dev/null 2>&1
来源：http://hz.wangshuangyany.cn/gtagrazwus.html

[R42] 输入重定向
来源：http://hz.0kj1m.cn/gtneyvoybh.html

wc -l < a.txt
来源：http://hz.tian-w.cn/gtjvxpkiob.html

[R43] 按名字查找文件
来源：http://hz.hfpthk.cn/gtrthiboxm.html

find . -name "*.log" -type f
来源：http://hz.dianchejie.cn/gtisfzvnoy.html

[R44] 按修改时间查找
来源：http://hz.shzxlz.cn/gtteirqghv.html

find . -mtime -7 -type f
来源：http://hz.shangyingyoupin.top/gtmwtyibjb.html

[R45] 批量删除
来源：http://hz.cucudq.cn/gtjoeayvdr.html

find . -name "*.tmp" -delete
来源：http://hz.bjfxy.top/gtjgnkzplb.html

[R46] 递归替换文件内容
来源：http://hz.yj20258.top/gtgbuvwwaf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.9152youxi.cn/gtqehmbiat.html

[R47] sed 单行替换
来源：http://hz.ivvv.top/gttamhfwfs.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shuidangran.top/gtgjysgubx.html

[R48] awk 取指定列
来源：http://hz.shangyingyoupin.top/gtzvmtlahe.html

awk '{print $1, $3}' a.txt
来源：http://hz.yonumen.top/gtrumdekzf.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gttwhdunbb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.dashuyun.cn/gtuyfbuljx.html

[R50] awk 求和
来源：http://hz.shanyushiyangkeji.top/gtbuxubzzl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cucudq.cn/gtjsrddvcy.html

[R51] 排序去重取前几
来源：http://hz.smart0.xyz/gtnjmiczxt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nwbrower.top/gtfoodkvkp.html

[R52] 统计行数
来源：http://hz.quarkkingdee.top/gtjdftrcoh.html

wc -l a.txt
来源：http://hz.iojbl.cn/gtgdoeymqk.html

[R53] 查看文件头与实时尾
来源：http://hz.jinghuilouyu.cn/gthtpzgjyd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ivvv.top/gtgegthpnr.html

[R54] 比较两个文件
来源：http://hz.nanxinkj.top/gthdmpwfgv.html

diff a.txt b.txt
来源：http://hz.zhixingplan.top/gtccbcrjbb.html

[R55] 压缩与解压
来源：http://hz.316326.xyz/gtcajqrfzz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jqgfzy.top/gtujtcktbn.html

[R56] 远程拷贝
来源：http://hz.jianghu66.top/gticwrksxl.html

scp file user@host:/path/
来源：http://hz.hywenlv.cn/gtcsgqaikq.html

[R57] 远程执行命令
来源：http://hz.nwbrower.top/gtjniukkem.html

ssh user@host 'uptime'
来源：http://hz.dianchejie.cn/gtvkbpkqpx.html

[R58] 下载文件
来源：http://hz.jinqigfzy.top/gthrmwbrba.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.redwolf501.top/gtxzwekaay.html

[R59] 发 POST JSON
来源：http://hz.hongshengwenyu.top/gtirudfovc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zycfv.cn/gtmlamntez.html

[R60] 只看 HTTP 状态码
来源：http://hz.jyoumei.cn/gttrmqejki.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.meibo888.top/gtkobtrdzq.html

[R61] 磁盘占用
来源：http://hz.jianghu66.top/gtzlepgfzw.html

df -h;  du -sh *
来源：http://hz.ywan-chungtsiang.top/gtctwcjobp.html

[R62] 找最占空间的文件
来源：http://hz.316326.xyz/gtwkbaqcpd.html

du -ah . | sort -rh | head -10
来源：http://hz.tian-w.cn/gtxdcjzcmk.html

[R63] 内存与进程
来源：http://hz.xinyue.icu/gthctqtqwy.html

free -h;  ps aux | grep nginx
来源：http://hz.yonumen.top/gtvlcclpnd.html

[R64] 结束进程
来源：http://hz.0kj1m.cn/gtndlmwqba.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenlongwang.top/gtqbohndqa.html

[R65] 查看端口占用
来源：http://hz.c1oappe.top/gtacizprcc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.dianchejie.cn/gtobgvbnpw.html

[R66] 定时任务
来源：http://hz.yvedp.cn/gtbgcijfpj.html

crontab -e;  crontab -l
来源：http://hz.sysykeji.top/gtfqtvjnkj.html

[R67] 生成随机十六进制串
来源：http://hz.zhijiandao.cn/gtonrmunwf.html

openssl rand -hex 16
来源：http://hz.hywenlv.cn/gtsffbsorg.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangkeji.top/gtrmebxaeg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shuidangran.top/gtiyspqgxg.html

[R69] 生成随机密码
来源：http://hz.ydzc1.top/gtplxtuqkx.html

head -c 16 /dev/urandom | base64
来源：http://hz.yongpay.top/gtvycczimw.html

[R70] 时间戳与互转
来源：http://hz.chenzaomai.com/gtkrudfobp.html

date +%s;  date -d @1700000000
来源：http://hz.cqqwz.cn/gttzjtgyux.html

[R71] 日期格式化
来源：http://hz.shangyingyoupin.top/gtkvfraipu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pengpengdd.cyou/gtwcxanril.html

[R72] 等待端口就绪
来源：http://hz.gaohongyu789.top/gtnyayjqez.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ehwqpu.com/gtfcuehpcw.html

[R73] 分割大日志
来源：http://hz.fengsongda.top/gtmetxztuz.html

split -l 1000 big.log part_
来源：http://hz.shangyingyoupin.top/gtmnerydzu.html

[R74] 批量重命名
来源：http://hz.ydzc1.top/gtwyhoanmt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenzaomai.com/gtdhhobvos.html

[R75] 导出环境变量
来源：http://hz.316326.xyz/gtampuhwwf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.feifeiyinyue.top/gtoyfvljek.html

[R76] 使用临时文件
来源：http://hz.meibo888.top/gtmwmzwccv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydzc1.top/gtjcodpoqy.html

[R77] 读取用户输入
来源：http://hz.jqgfzy.top/gtmqphbppy.html

read -rp "请输入: " ans
来源：http://hz.zhaomingkeji.xyz/gtstguyvpa.html

[R78] 交互式菜单
来源：http://hz.jlsjyb.cn/gtffmjwoip.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shangyingyoupin.top/gtigamqcim.html

[R79] 解析命令行选项
来源：http://hz.sysykeji.top/gtyryitgub.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xziqi.cn/gtjcvkfate.html

[R80] 查看脚本执行耗时
来源：http://hz.yangfankeji.com/gtmllxlbtc.html

time ./run.sh
来源：http://hz.yj20258888.top/gtvopuvlmp.html

================================================================================
来源：http://hz.quarkkingdee.top/gtenkkcazz.html

S. C / C++ 专题
来源：http://hz.shanyushiyangtech.top/gtyvtipati.html

================================================================================
来源：http://hz.yanxiufei.cn/gtdvpugfgp.html

[S01] C：Hello World
来源：http://hz.jinqigfzy.top/gtughnkewp.html

#include <stdio.h>
来源：http://hz.yj20258888.top/gtvdlfutvo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhiwuduotai.top/gtbotxcaeb.html

[S02] C：变量与格式化输出
来源：http://hz.zhongyouzk.top/gtqqztzijs.html

int a = 10; printf("%d\n", a);
来源：http://hz.feifeiyinyue.top/gtakiuybtt.html

[S03] C：读入整数
来源：http://hz.quarkkingdee.top/gtibmqugdd.html

int x; scanf("%d", &x);
来源：http://hz.tianlin.xyz/gtqoijrwfa.html

[S04] C：字符串复制
来源：http://hz.tian-w.cn/gtkkukxkqc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hammf.cn/gtgsulrglh.html

[S05] C：字符串长度
来源：http://hz.fzhhl.top/gtyisymbjz.html

strlen(s)
来源：http://hz.chenlongwang.top/gtugyydepe.html

[S06] C：字符串比较
来源：http://hz.yueranfly.top/gtyhszchxm.html

strcmp(a, b) == 0
来源：http://hz.shzxlz.cn/gtqzxnzaec.html

[S07] C：数组遍历求和
来源：http://hz.yvedp.cn/gtujpuxptq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xziqi.cn/gtcdlovwdw.html

[S08] C：动态内存分配与释放
来源：http://hz.dianchejie.cn/gtniacxcau.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.meibo888.top/gttqnafuoj.html

[S09] C：结构体定义与初始化
来源：http://hz.feifeiyinyue.top/gtdjoprzju.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sysykeji.top/gtwplxrhkn.html

[S10] C：指针与解引用
来源：http://hz.xinyue.icu/gtslrujsdy.html

int *p = &a;  *p = 5;
来源：http://hz.sysykeji.top/gtpjpgzjoz.html

[S11] C：逐行读文件
来源：http://hz.andypj.xyz/gtspuzdqod.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.guannengcc.top/gteqjgiofa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.dashuyun.cn/gtwleqjenk.html

fclose(f);
来源：http://hz.hammf.cn/gtogdlmclj.html

[S12] C：写文件
来源：http://hz.mhx1999.top/gtwfzhljet.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.fengsongda.top/gtpngzcwxc.html

[S13] C：宏定义
来源：http://hz.guowangkeji.top/gtqsxlxgqm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj20258.top/gttgqfrwcl.html

[S14] C：枚举
来源：http://hz.hammf.cn/gtdyqunttm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tanke756.top/gtcmacplmo.html

[S15] C：类型转换
来源：http://hz.jqgufenzy.top/gtkpzgahiy.html

(double) a / b
来源：http://hz.quarkkingdee.top/gtknzeqxbv.html

[S16] C：位操作置位
来源：http://hz.chenjidiqi.icu/gtzaxpjufn.html

x |= (1 << 3);
来源：http://hz.xuetiantiany.cn/gtwpkcnafa.html

[S17] C：安全拼接字符串
来源：http://hz.cucudq.cn/gtzqsunhho.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangshuangyany.cn/gtarqjpzlz.html

[S18] C：命令行参数
来源：http://hz.zhaomingkeji.xyz/gtqowpmrar.html

int main(int argc, char **argv)
来源：http://hz.0kj1m.cn/gtdxouvbhe.html

[S19] C：快速排序
来源：http://hz.yuanzhike.top/gtfdbndfxs.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhengqikj.top/gtolmwnmgu.html

[S20] C：二分查找
来源：http://hz.gotoacloud.top/gthcstqfwq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ppjwa.cn/gttpsckxfg.html

[S21] C：字符类别判断
来源：http://hz.ehwqpu.com/gtwmisydqi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinghuilouyu.cn/gtufkvwuhe.html

[S22] C：字符串转数字
来源：http://hz.ybcxt.top/gtvgjyoojd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nanxuanxn.top/gtrukljmvq.html

[S23] C：随机数
来源：http://hz.vqdsnc.cn/gtpsgcbknw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.52xcode.cn/gtcyybkwso.html

[S24] C：获取本地时间
来源：http://hz.zhiwuduotai.top/gtzcaetsur.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hywenlv.cn/gtckubhakk.html

[S25] C：内存拷贝
来源：http://hz.gzhubu.top/gtvswzxxui.html

memcpy(dst, src, n);
来源：http://hz.haohaochexian.top/gtmadzxsca.html

[S26] C：内存清零
来源：http://hz.nanxinkj.top/gtzwdnkrhq.html

memset(a, 0, sizeof a);
来源：http://hz.zhongyouzk.top/gtwncccezr.html

[S27] C：定义常量
来源：http://hz.tian-w.cn/gtqbrjfejs.html

const double PI = 3.14159;
来源：http://hz.ppjwa.cn/gtjtrjglar.html

[S28] C：静态变量
来源：http://hz.xingfuxueyuan.xyz/gteyrpjqqw.html

static int counter = 0;
来源：http://hz.jqgufenzy.top/gtynvsgxrf.html

[S29] C：变参函数
来源：http://hz.jqgfzy.top/gtujuigylu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yongpay.top/gtznxnmcvm.html

[S30] C：头文件保护
来源：http://hz.meibo888.top/gtxgbihplm.html

#ifndef X_H
来源：http://hz.jinqigfzy.top/gtwfffbtds.html

#define X_H
来源：http://hz.yj20258888.top/gtcucoykmu.html

#endif
来源：http://hz.gogol.net.cn/gtqrakfljk.html

[S31] C++：Hello World
来源：http://hz.jinqigufen.top/gtiviodrkw.html

#include <iostream>
来源：http://hz.shangyingyoupin.top/gtrlfgrpta.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenzaomai.com/gtgukzjmli.html

[S32] C++：字符串
来源：http://hz.mhx1999.top/gtqbkuszha.html

std::string s = "hi";  s += "!";
来源：http://hz.mhx1999.top/gtcdirswvw.html

[S33] C++：vector 增删
来源：http://hz.chenlongwang.top/gtmdjblglj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pycfn.com/gtdaqtwigv.html

[S34] C++：遍历 vector
来源：http://hz.pycfn.com/gttfupogys.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shzxlz.cn/gtnaqbwqhz.html

[S35] C++：map
来源：http://hz.ivvv.top/gtfdckhqql.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtspqpxtgr.html

[S36] C++：unordered_map
来源：http://hz.ivvv.top/gtyicncphe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtisozmhil.html

[S37] C++：set
来源：http://hz.tian-w.cn/gthwqisrza.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aibaodan.cn/gtimtlwiio.html

[S38] C++：排序
来源：http://hz.shanyushiyangkeji.top/gtbtycktns.html

std::sort(v.begin(), v.end());
来源：http://hz.xuanzx.com/gtscdkxfhc.html

[S39] C++：自定义比较器排序
来源：http://hz.feifeiyinyue.top/gtdewwvytk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zdqjudy.top/gttpdwiurc.html

[S40] C++：查找元素
来源：http://hz.zycfv.cn/gtpllcazyb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xuanzx.com/gtyynjaxzh.html

[S41] C++：类与构造函数
来源：http://hz.yueranfly.top/gtyhbpwixi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258888.top/gtrnyodtfj.html

[S42] C++：继承与虚函数
来源：http://hz.316326.xyz/gtcqtjifri.html

class B : public Base { public: void f() override {} };
来源：http://hz.hywenlv.cn/gtcptktady.html

[S43] C++：智能指针
来源：http://hz.cqqwz.cn/gtlisxphuu.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnqzz.top/gtvsedradj.html

[S44] C++：引用传参
来源：http://hz.wangshuangyany.cn/gteyueoisk.html

void inc(int &x) { ++x; }
来源：http://hz.iojbl.cn/gtgcrgavbl.html

[S45] C++：lambda
来源：http://hz.sxryk.cn/gtbxmccoit.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinyuanbaomall.cn/gtangjvbkl.html

[S46] C++：函数模板
来源：http://hz.zhijiandao.cn/gtdpakrptj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jiagoushi.top/gtigjvusvj.html


<!-- 参考信息 -->