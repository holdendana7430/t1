代发 wailian999

SHOW INDEX FROM users;
来源：http://hz.dianchejie.cn/gtffxjovnu.html

[Q73] 查看表状态
来源：http://hz.snrcjt.cn/gtqvgexfvi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jqgfzy.top/gthmlpvjva.html

[Q74] 强制使用索引
来源：http://hz.shanyushiyangtech.top/gtlckdpbfj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gtucmgmhut.html

[Q75] 日期格式化
来源：http://hz.hnxiangtu.top/gtykpnpdwr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.nanxuanxn.top/gtpeluyvqs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.c1oappe.top/gtoqctnavc.html

[Q76] 按天统计
来源：http://hz.snrcjt.cn/gtteevauon.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinyuanbaomall.cn/gtolcrzkxs.html

[Q77] 时间加减
来源：http://hz.dianchejie.cn/gtkckuchaj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.redwolf501.top/gtzjfxbshb.html

[Q78] 当前时间
来源：http://hz.ivvv.top/gtrajhfibl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxinkj.top/gtukomsmcn.html

[Q79] 字符串拼接
来源：http://hz.kuanghao11.cn/gtjojykdyg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yvedp.cn/gtqhalijex.html

[Q80] 字符串截取
来源：http://hz.jqgfzy.top/gtxdqyeyin.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hysaishi.cn/gtzgzfeowk.html

[Q81] 字符串替换
来源：http://hz.jinqigfzy.top/gtmlcmxvbw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnxiangtu.top/gtrdtrzsic.html

[Q82] 字符长度与字节长度
来源：http://hz.zdqjudy.top/gtkbfjkglb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.vqdsnc.cn/gtfiezegjv.html

[Q83] 大小写转换
来源：http://hz.hysaishi.cn/gtoacxfure.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtlpuwojsz.html

[Q84] 去除首尾空格
来源：http://hz.aibaodan.cn/gtmmbfprsi.html

SELECT TRIM(name) FROM users;
来源：http://hz.haohaochexian.top/gtwlrvwngw.html

[Q85] 数值取整
来源：http://hz.gzhubu.top/gteihhsrjt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.fzhhl.top/gtcnxaftwa.html

[Q86] 读取 JSON 字段
来源：http://hz.yueranfly.top/gtosjqroey.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258888.top/gtgloppddh.html

[Q87] JSON 字段做条件
来源：http://hz.cheryme.top/gtzljqpyod.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.fengsongda.top/gtckhvpkdl.html

[Q88] 行转列（条件聚合）
来源：http://hz.cdnleiting.top/gtcwimgugj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xylfe.cn/gtqurtaltq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sysykeji.top/gtkrztmzdz.html

[Q89] 判断表是否存在
来源：http://hz.hfpthk.cn/gtqomkjczo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xziqi.cn/gtbpjiwpln.html

[Q90] 生成序号列
来源：http://hz.316326.xyz/gtbvedotvc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pengpengdd.cyou/gtfesmhiag.html

================================================================================
来源：http://hz.gogol.net.cn/gtplufgcen.html

R. Bash 专题
来源：http://hz.gzhubu.top/gtgrnkzxll.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtypbgvylm.html

[R01] shebang 与严格模式
来源：http://hz.jinghuilouyu.cn/gthaxrjrpw.html

#!/usr/bin/env bash
来源：http://hz.tianlin.xyz/gtjrrfnwwa.html

set -euo pipefail
来源：http://hz.sysykeji.top/gtcbsahnvr.html

[R02] 变量赋值与使用
来源：http://hz.bjfxy.top/gtxlaaulvp.html

name="Tom"; echo "$name"
来源：http://hz.daria6918.cn/gtairccjkz.html

[R03] 只读变量
来源：http://hz.ybcxt.top/gtancvtvkk.html

readonly PI=3.14
来源：http://hz.aizwys.cn/gtxzzraaoy.html

[R04] 位置参数
来源：http://hz.dashuyun.cn/gtxnvllols.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nwbrower.top/gtnypbgsqz.html

[R05] 参数默认值
来源：http://hz.jinyuanbaomall.cn/gtprbrjckq.html

name="${1:-default}"
来源：http://hz.zycfv.cn/gtvjmhisgn.html

[R06] 判断命令是否存在
来源：http://hz.52xcode.cn/gtnxragvth.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hysaishi.cn/gtjrssazdn.html

[R07] if 判断文件
来源：http://hz.wangshuangyany.cn/gtxqnhchqv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xylfe.cn/gtgicmofvb.html

[R08] 数值比较
来源：http://hz.cucudq.cn/gtokseqppb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jianghu66.top/gtogsoijca.html

[R09] 字符串比较
来源：http://hz.chenjidiqi.icu/gtxjpuqjhz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hnqzz.top/gtfabbhdel.html

[R10] 正则匹配
来源：http://hz.hammf.cn/gtjeyubacn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tian-w.cn/gtojkfuyls.html

[R11] case 多分支
来源：http://hz.yangfankeji.com/gtyitwtfti.html

case "$1" in
来源：http://hz.dashuyun.cn/gtoaddmruu.html

start) echo "启动" ;;
来源：http://hz.zhaomingkeji.xyz/gtomdzlcwz.html

stop)  echo "停止" ;;
来源：http://hz.hongshengwenyu.top/gtabgtvgcw.html

*)     echo "未知命令" ;;
来源：http://hz.feifeiyinyue.top/gtwtqhcoux.html

esac
来源：http://hz.dianchejie.cn/gtxwgojzvu.html

[R12] for 遍历文件
来源：http://hz.feifeiyinyue.top/gtkzoyovzs.html

for f in *.txt; do echo "$f"; done
来源：http://hz.mhx1999.top/gtnxyqealz.html

[R13] for 计数循环
来源：http://hz.jinqigufen.top/gtfuikhunz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtfvoirnxl.html

[R14] C 风格 for
来源：http://hz.gzhubu.top/gtqqqetmoq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ydjk.org.cn/gtlrsfwjpa.html

[R15] while 逐行读文件
来源：http://hz.sufxvd.cn/gtbrjbgmix.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daria6918.cn/gtoajbiewt.html

[R16] until 等待条件
来源：http://hz.0kj1m.cn/gtjskpynul.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xuanzx.com/gtflnpkmns.html

[R17] 数组定义与取值
来源：http://hz.wangshuangyany.cn/gtktcrznfk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.quarkkingdee.top/gtsnjwepyh.html

[R18] 遍历数组
来源：http://hz.zhengqikj.top/gttcytuobe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.mhx1999.top/gtrhxyeqaq.html

[R19] 数组长度
来源：http://hz.sxryk.cn/gtikirhxao.html

echo "${#arr[@]}"
来源：http://hz.ybcxt.top/gtciimgogz.html

[R20] 关联数组（字典）
来源：http://hz.wangshuangyany.cn/gtpetttqsx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cqqwz.cn/gtrufzyqrb.html

[R21] 字符串长度
来源：http://hz.fengsongda.top/gtrcfqfptt.html

echo "${#s}"
来源：http://hz.vqdsnc.cn/gtpvxasuwi.html

[R22] 截取子串
来源：http://hz.chenjidiqi.icu/gtedgnytty.html

echo "${s:0:5}"
来源：http://hz.quarkkingdee.top/gtcpaalqbi.html

[R23] 字符串替换
来源：http://hz.aibaodan.cn/gtdhdgffga.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xziqi.cn/gtswnsdajo.html

[R24] 大小写转换
来源：http://hz.zycfv.cn/gtpdwvembg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.quarkkingdee.top/gtuowukwbw.html

[R25] 去后缀 / 去前缀
来源：http://hz.feifeiyinyue.top/gtirzyvuay.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fzhhl.top/gthoevmifz.html

[R26] 命令替换
来源：http://hz.meibo888.top/gtxwgoxqfj.html

now=$(date +%F); echo "$now"
来源：http://hz.vqdsnc.cn/gtzhydalxs.html

[R27] 算术展开
来源：http://hz.wangdashe.top/gtulmyzral.html

echo $((1 + 2 * 3))
来源：http://hz.zhoulong.xyz/gtjbinrjvm.html

[R28] 浮点运算
来源：http://hz.wangshuangyany.cn/gtuvdsbrqs.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangkeji.top/gttxwgvobq.html

[R29] 定义函数
来源：http://hz.guowangkeji.top/gtphsvcgqp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.pycfn.com/gtamatnbqi.html

[R30] 函数返回状态码
来源：http://hz.nwbrower.top/gtvlwqppkd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xinyue.icu/gtwrznhstv.html

[R31] 局部变量
来源：http://hz.gotoacloud.top/gtqbgzaikc.html

f() { local x=1; echo "$x"; }
来源：http://hz.xuanzx.com/gtqplyaakp.html

[R32] 参数个数校验
来源：http://hz.chenjidiqi.icu/gthpszyqqt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jlsjyb.cn/gtsngwnhbf.html

[R33] 捕获错误并提示行号
来源：http://hz.zhiwuduotai.top/gtvvmohgfn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenlongwang.top/gtrufeybpc.html

[R34] 退出时清理
来源：http://hz.yj20258888.top/gtawewgnyv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tanke756.top/gtjphtsgqt.html

[R35] 后台执行并等待
来源：http://hz.jiagoushi.top/gtapcldtsq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.aibaodan.cn/gtpcjchnea.html

[R36] 并发执行多个任务
来源：http://hz.gogol.net.cn/gtacauxylb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.vqdsnc.cn/gtvumfqfwi.html

[R37] 把输出赋给变量
来源：http://hz.quarkkingdee.top/gtokalguvb.html

files=$(ls -1)
来源：http://hz.nanxinkj.top/gtvdohezqu.html

[R38] 管道串联
来源：http://hz.aizwys.cn/gtdtwwnwge.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xinyue.icu/gtgvtdzjta.html

[R39] 重定向标准输出与错误
来源：http://hz.cdnleiting.top/gtdloqjkma.html

cmd > out.log 2>&1
来源：http://hz.birdmap.top/gtygyauzwg.html

[R40] 追加写日志
来源：http://hz.sysykeji.top/gtqswoxeti.html

echo "log" >> out.log
来源：http://hz.zhengqikj.top/gtmidmnhlh.html

[R41] 丢弃输出
来源：http://hz.gaohongyu789.top/gtkadsrtkr.html

cmd >/dev/null 2>&1
来源：http://hz.yangfankeji.com/gtwzbroodx.html

[R42] 输入重定向
来源：http://hz.jinqigufen.top/gtrzugmwqc.html

wc -l < a.txt
来源：http://hz.hywenlv.cn/gtwxqoynov.html

[R43] 按名字查找文件
来源：http://hz.jinqigfzy.top/gtqfkmkbys.html

find . -name "*.log" -type f
来源：http://hz.fengsongda.top/gtkwlzqghf.html

[R44] 按修改时间查找
来源：http://hz.fzhhl.top/gtalnjzcfy.html

find . -mtime -7 -type f
来源：http://hz.daxiang520.top/gtontdrrxz.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gtfauoultr.html

find . -name "*.tmp" -delete
来源：http://hz.daria6918.cn/gtylkdxslz.html

[R46] 递归替换文件内容
来源：http://hz.mhx1999.top/gtrtbmgpkg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xingfuxueyuan.xyz/gtiqkdgpdl.html

[R47] sed 单行替换
来源：http://hz.shzxlz.cn/gtgoukivgw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fengsongda.top/gtyswhffqj.html

[R48] awk 取指定列
来源：http://hz.wangshuangyany.cn/gtxwnxhcty.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhengqikj.top/gtahkkmxns.html

[R49] awk 带条件
来源：http://hz.pycfn.com/gtrjcdmoai.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jiagoushi.top/gtczkhxrmo.html

[R50] awk 求和
来源：http://hz.hongshengwenyu.top/gtbxwxkywb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.fengsongda.top/gtorrvlrcm.html

[R51] 排序去重取前几
来源：http://hz.svipenyu.cn/gtafpgitjl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ehwqpu.com/gtlrdkrpej.html

[R52] 统计行数
来源：http://hz.ydzc1.top/gtphmypdmh.html

wc -l a.txt
来源：http://hz.redwolf501.top/gtyjtgdinw.html

[R53] 查看文件头与实时尾
来源：http://hz.gotoacloud.top/gtclgetafb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yvedp.cn/gtmkawyqde.html

[R54] 比较两个文件
来源：http://hz.fengsongda.top/gtcrggusja.html

diff a.txt b.txt
来源：http://hz.zhixingplan.top/gtnsrtlblr.html

[R55] 压缩与解压
来源：http://hz.shuidangran.top/gtgqpxwfny.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yuanzhike.top/gtzfcxmuqe.html

[R56] 远程拷贝
来源：http://hz.ivvv.top/gtkwptdngg.html

scp file user@host:/path/
来源：http://hz.xziqi.cn/gtgutkawuo.html

[R57] 远程执行命令
来源：http://hz.gogol.net.cn/gtvdowrcrv.html

ssh user@host 'uptime'
来源：http://hz.vqdsnc.cn/gtqxyrjtru.html

[R58] 下载文件
来源：http://hz.iojbl.cn/gtcvibwtor.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.redwolf501.top/gtaggapdjb.html

[R59] 发 POST JSON
来源：http://hz.jqgfzy.top/gtoznflntt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.fengsongda.top/gtmlrueocx.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtjrgmboam.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhengqikj.top/gtydugxsmn.html

[R61] 磁盘占用
来源：http://hz.yueranfly.top/gtmvjwbgsi.html

df -h;  du -sh *
来源：http://hz.hywenlv.cn/gtaayromse.html

[R62] 找最占空间的文件
来源：http://hz.wangshuangyany.cn/gtgrtohhrh.html

du -ah . | sort -rh | head -10
来源：http://hz.snrcjt.cn/gtvwqlcenv.html

[R63] 内存与进程
来源：http://hz.shanyushiyangkeji.top/gtkdrupuit.html

free -h;  ps aux | grep nginx
来源：http://hz.mhx1999.top/gtkzokhzdw.html

[R64] 结束进程
来源：http://hz.hnxiangtu.top/gtvsypawwg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yuxming.cn/gtahxzebik.html

[R65] 查看端口占用
来源：http://hz.haohaochexian.top/gtnsgjtbnh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.bjfxy.top/gtxqljhylg.html

[R66] 定时任务
来源：http://hz.xinyue.icu/gtxygdykhk.html

crontab -e;  crontab -l
来源：http://hz.zycfv.cn/gtgzmgwzpb.html

[R67] 生成随机十六进制串
来源：http://hz.52xcode.cn/gtcdkerjks.html

openssl rand -hex 16
来源：http://hz.nanxuanxn.top/gttyvhhkda.html

[R68] 计算文件校验值
来源：http://hz.shuidangran.top/gtzscalafl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.haohaochexian.top/gtmmtnjqqb.html

[R69] 生成随机密码
来源：http://hz.aibaodan.cn/gtpwdytrbu.html

head -c 16 /dev/urandom | base64
来源：http://hz.jqgfzy.top/gtnvifxzoq.html

[R70] 时间戳与互转
来源：http://hz.hnxiangtu.top/gthveekkgc.html

date +%s;  date -d @1700000000
来源：http://hz.zdqjudy.top/gtaldfkpvl.html

[R71] 日期格式化
来源：http://hz.nanxinkj.top/gtlxxmhzer.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.birdmap.top/gthbxvjwhf.html

[R72] 等待端口就绪
来源：http://hz.jqgufenzy.top/gtichnvztm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtjnrboztb.html

[R73] 分割大日志
来源：http://hz.shuidangran.top/gtwirjnwnp.html

split -l 1000 big.log part_
来源：http://hz.0kj1m.cn/gtsgdskouv.html

[R74] 批量重命名
来源：http://hz.yj202588.top/gtuhwoxiny.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xziqi.cn/gtysdffkop.html

[R75] 导出环境变量
来源：http://hz.zhixingplan.top/gtkstlkfua.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hnqzz.top/gtijhbioqm.html

[R76] 使用临时文件
来源：http://hz.zhengqikj.top/gtzhibqftq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtgpkaweqd.html

[R77] 读取用户输入
来源：http://hz.dianchejie.cn/gtqsnzsbya.html

read -rp "请输入: " ans
来源：http://hz.redwolf501.top/gtryszkseu.html

[R78] 交互式菜单
来源：http://hz.redwolf501.top/gthqioatds.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xingfuxueyuan.xyz/gtsjonskwy.html

[R79] 解析命令行选项
来源：http://hz.yj20258888.top/gtrklxvcma.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhixingplan.top/gthksnszpo.html

[R80] 查看脚本执行耗时
来源：http://hz.guowangkeji.top/gtvgzcasem.html

time ./run.sh
来源：http://hz.quarkkingdee.top/gtwokencfn.html

================================================================================
来源：http://hz.xylfe.cn/gtwadgbwfs.html

S. C / C++ 专题
来源：http://hz.xuanzx.com/gtjfayjsgs.html

================================================================================
来源：http://hz.aibaodan.cn/gtdscvebny.html

[S01] C：Hello World
来源：http://hz.gogol.net.cn/gtmjefriff.html

#include <stdio.h>
来源：http://hz.cashguo.top/gtzrygzrfi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gzhubu.top/gtakcwhoty.html

[S02] C：变量与格式化输出
来源：http://hz.smart0.xyz/gtpwxhtyvy.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinghuilouyu.cn/gtvgsihbcd.html

[S03] C：读入整数
来源：http://hz.guowangkeji.top/gtpyxsacvi.html

int x; scanf("%d", &x);
来源：http://hz.chenzaomai.com/gthlnmmoqq.html

[S04] C：字符串复制
来源：http://hz.yj20258.top/gtggwzihwn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sxryk.cn/gtcqrpkobg.html

[S05] C：字符串长度
来源：http://hz.havefunace.top/gtjhzscrfd.html

strlen(s)
来源：http://hz.sufxvd.cn/gtveqmgbsy.html

[S06] C：字符串比较
来源：http://hz.nanxuanxn.top/gtbhuxkoyy.html

strcmp(a, b) == 0
来源：http://hz.shzxlz.cn/gtrxeczgks.html

[S07] C：数组遍历求和
来源：http://hz.xziqi.cn/gtexiyaquu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xinyue.icu/gtsgnpjgsw.html

[S08] C：动态内存分配与释放
来源：http://hz.cdnleiting.top/gtccqzlrhw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.aibaodan.cn/gtzyhfrlrg.html

[S09] C：结构体定义与初始化
来源：http://hz.sweek.top/gtnltjxcyx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yanxiufei.cn/gtlhyqrlad.html

[S10] C：指针与解引用
来源：http://hz.yanxiufei.cn/gtyuzkxbxh.html

int *p = &a;  *p = 5;
来源：http://hz.ybcxt.top/gthobnqqpa.html

[S11] C：逐行读文件
来源：http://hz.hysaishi.cn/gtfqxqxstm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.daxiang520.top/gtfhmczqjg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.guowangkeji.top/gtprilhkou.html

fclose(f);
来源：http://hz.sxryk.cn/gtnwnzwmpl.html

[S12] C：写文件
来源：http://hz.jinqigufen.top/gtimmphxgm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.mhx1999.top/gtgaseqbsd.html

[S13] C：宏定义
来源：http://hz.dashuyun.cn/gtlqudceri.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.dianchejie.cn/gtbtymwivx.html

[S14] C：枚举
来源：http://hz.hysaishi.cn/gtikxhurpv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jiagoushi.top/gtgugnwmhv.html

[S15] C：类型转换
来源：http://hz.meibo888.top/gtvgbeadpb.html

(double) a / b
来源：http://hz.havefunace.top/gtdeejmypw.html

[S16] C：位操作置位
来源：http://hz.hammf.cn/gtbztwawff.html

x |= (1 << 3);
来源：http://hz.hammf.cn/gtbkdejdau.html

[S17] C：安全拼接字符串
来源：http://hz.havefunace.top/gtepkdxsjm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydjk.org.cn/gtclxalofz.html

[S18] C：命令行参数
来源：http://hz.daxiang520.top/gtwazgoity.html

int main(int argc, char **argv)
来源：http://hz.xziqi.cn/gtkzkxozsi.html

[S19] C：快速排序
来源：http://hz.vqdsnc.cn/gtscfioizs.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yanxiufei.cn/gtkqahpmlt.html

[S20] C：二分查找
来源：http://hz.yangfankeji.com/gtrswwelmh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hfpthk.cn/gtatprpppo.html

[S21] C：字符类别判断
来源：http://hz.xuetiantiany.cn/gtsfcxmnrt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hywenlv.cn/gtonbkykqd.html

[S22] C：字符串转数字
来源：http://hz.pycfn.com/gtgjgqjboh.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhiwuduotai.top/gttxmgfanl.html

[S23] C：随机数
来源：http://hz.hammf.cn/gtoxhfxvli.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yj202588.top/gtxfknulow.html

[S24] C：获取本地时间
来源：http://hz.xylfe.cn/gtvmmjcxtn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xuetiantiany.cn/gtylncjgbx.html

[S25] C：内存拷贝
来源：http://hz.sysykeji.top/gtclmnkydp.html

memcpy(dst, src, n);
来源：http://hz.chenjidiqi.icu/gtpeciaegy.html

[S26] C：内存清零
来源：http://hz.cashguo.top/gtpdzuxfin.html

memset(a, 0, sizeof a);
来源：http://hz.aibaodan.cn/gtmkkbetok.html

[S27] C：定义常量
来源：http://hz.fengsongda.top/gtdxsntdxs.html

const double PI = 3.14159;
来源：http://hz.cheryme.top/gtfvkrgjli.html

[S28] C：静态变量
来源：http://hz.jqgufenzy.top/gtofxturva.html

static int counter = 0;
来源：http://hz.cucudq.cn/gtayaetjhx.html

[S29] C：变参函数
来源：http://hz.iojbl.cn/gtdbfkxkag.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.pengpengdd.cyou/gtisbjyldr.html

[S30] C：头文件保护
来源：http://hz.hongshengwenyu.top/gtsvphmvbk.html

#ifndef X_H
来源：http://hz.yueranfly.top/gtxrxxzfpr.html

#define X_H
来源：http://hz.yuxming.cn/gticqfaokd.html

#endif
来源：http://hz.chenzaomai.com/gtovzrleje.html

[S31] C++：Hello World
来源：http://hz.nanxuanxn.top/gtpezidqrm.html

#include <iostream>
来源：http://hz.0kj1m.cn/gtzrwtswuj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jlsjyb.cn/gtnalrfjax.html

[S32] C++：字符串
来源：http://hz.pycfn.com/gtzkbmqwbp.html

std::string s = "hi";  s += "!";
来源：http://hz.pycfn.com/gtnglkhxgz.html

[S33] C++：vector 增删
来源：http://hz.gogol.net.cn/gtzunfllkc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hfpthk.cn/gtnmxwvbsv.html

[S34] C++：遍历 vector
来源：http://hz.svipenyu.cn/gtxbzhzvma.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fzhhl.top/gtbsptsvmx.html

[S35] C++：map
来源：http://hz.chenjidiqi.icu/gtyxwozmsl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtlazooiuw.html

[S36] C++：unordered_map
来源：http://hz.zhengqikj.top/gthakteens.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtpsdhedvz.html

[S37] C++：set
来源：http://hz.chenjidiqi.icu/gtqmahislk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.guowangkeji.top/gtykwhpjml.html

[S38] C++：排序
来源：http://hz.xuanzx.com/gtjruozaia.html

std::sort(v.begin(), v.end());
来源：http://hz.iojbl.cn/gtsaqfqsqd.html

[S39] C++：自定义比较器排序
来源：http://hz.daxiang520.top/gtmztbxusd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ehwqpu.com/gtaffvhric.html

[S40] C++：查找元素
来源：http://hz.hysaishi.cn/gtlesceszo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gaohongyu789.top/gtcfgrobpc.html

[S41] C++：类与构造函数
来源：http://hz.jinyuanbaomall.cn/gtlgeacwii.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.smart0.xyz/gtrxhlzfwb.html

[S42] C++：继承与虚函数
来源：http://hz.ydzc1.top/gtbyvqnaos.html

class B : public Base { public: void f() override {} };
来源：http://hz.cdnleiting.top/gtoejjsbhp.html


<!-- 参考信息 -->