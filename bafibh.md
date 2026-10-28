代发 wailian999

ROLLBACK TO sp1;
来源：http://hz.daxiang520.top/gtpidebxfd.html

[Q69] 查看执行计划
来源：http://hz.jianghu66.top/gtjkdhnbmp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhijiandao.cn/gtrjiubhhm.html

[Q70] 更新统计信息
来源：http://hz.zhengqikj.top/gtkuczmbtb.html

ANALYZE TABLE users;
来源：http://hz.wangshuangyany.cn/gtwzifjogw.html

[Q71] 查看建表语句
来源：http://hz.zycfv.cn/gtuwrdpxhz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinyuanbaomall.cn/gtltfzzcte.html

[Q72] 查看索引
来源：http://hz.wangdashe.top/gtueyltbqw.html

SHOW INDEX FROM users;
来源：http://hz.pengpengdd.cyou/gtqhnwgtwm.html

[Q73] 查看表状态
来源：http://hz.feifeiyinyue.top/gtnoguffyx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dashuyun.cn/gtxduyyesj.html

[Q74] 强制使用索引
来源：http://hz.yongpay.top/gtqpqefypx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.smart0.xyz/gtqquxjurf.html

[Q75] 日期格式化
来源：http://hz.cucudq.cn/gtevifwsmg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daxiang520.top/gtqxbwsyaj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhoulong.xyz/gtzlybpdpo.html

[Q76] 按天统计
来源：http://hz.ydjk.org.cn/gtmzflimrc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenlongwang.top/gtzyeesfxc.html

[Q77] 时间加减
来源：http://hz.zycfv.cn/gthwsglcvq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gaohongyu789.top/gtzktrxita.html

[Q78] 当前时间
来源：http://hz.gotoacloud.top/gtnazlowje.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xuanzx.com/gtcoabodai.html

[Q79] 字符串拼接
来源：http://hz.jqgfzy.top/gtfyvjlazz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hysaishi.cn/gtubwxvozl.html

[Q80] 字符串截取
来源：http://hz.jyoumei.cn/gtplrlnver.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.snrcjt.cn/gtuefhvdrz.html

[Q81] 字符串替换
来源：http://hz.gaohongyu789.top/gtihiixfza.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cashguo.top/gtsugmljpe.html

[Q82] 字符长度与字节长度
来源：http://hz.xingfuxueyuan.xyz/gtiksjgicw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnxiangtu.top/gtypgtxqfm.html

[Q83] 大小写转换
来源：http://hz.zhoulong.xyz/gtiemnuzoc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.guannengcc.top/gtwobejhum.html

[Q84] 去除首尾空格
来源：http://hz.sxryk.cn/gtuyiaktmp.html

SELECT TRIM(name) FROM users;
来源：http://hz.hysaishi.cn/gtlxujyxab.html

[Q85] 数值取整
来源：http://hz.guannengcc.top/gtioeivnry.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinyuanbaomall.cn/gtynszxhbf.html

[Q86] 读取 JSON 字段
来源：http://hz.hysaishi.cn/gtfkonlcmn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.aizwys.cn/gtgcnvemrq.html

[Q87] JSON 字段做条件
来源：http://hz.pengpengdd.cyou/gtpsorbvcm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sysykeji.top/gtrucccpeq.html

[Q88] 行转列（条件聚合）
来源：http://hz.gogol.net.cn/gtiqnlpxul.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jiagoushi.top/gtnwhtqnra.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.fengsongda.top/gtpmuikvuu.html

[Q89] 判断表是否存在
来源：http://hz.mhx1999.top/gtbteypbdn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zdqjudy.top/gtpukfgemw.html

[Q90] 生成序号列
来源：http://hz.guowangkeji.top/gthaejycry.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.birdmap.top/gtdhniryhi.html

================================================================================
来源：http://hz.gogol.net.cn/gtmovlcejx.html

R. Bash 专题
来源：http://hz.sysykeji.top/gtikkaxlve.html

================================================================================
来源：http://hz.dashuyun.cn/gtsdfrdsib.html

[R01] shebang 与严格模式
来源：http://hz.zhixingplan.top/gtgkhzzqim.html

#!/usr/bin/env bash
来源：http://hz.smart0.xyz/gtqdhjtvzy.html

set -euo pipefail
来源：http://hz.aizwys.cn/gtgcxjxqfv.html

[R02] 变量赋值与使用
来源：http://hz.gzhubu.top/gtfxfbubmy.html

name="Tom"; echo "$name"
来源：http://hz.jinghuilouyu.cn/gtjxuborlx.html

[R03] 只读变量
来源：http://hz.hysaishi.cn/gtjnzzzxii.html

readonly PI=3.14
来源：http://hz.yangfankeji.com/gtgpmlpkox.html

[R04] 位置参数
来源：http://hz.jqgufenzy.top/gtrdeiwzuo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shuidangran.top/gtvooxbkfd.html

[R05] 参数默认值
来源：http://hz.bjfxy.top/gtssmzgxcx.html

name="${1:-default}"
来源：http://hz.iojbl.cn/gtzyqpixaw.html

[R06] 判断命令是否存在
来源：http://hz.andypj.xyz/gtzjnhkoaq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yueranfly.top/gtrjzhyxvl.html

[R07] if 判断文件
来源：http://hz.hammf.cn/gtrmwdkbwa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cheryme.top/gtrpozzlzs.html

[R08] 数值比较
来源：http://hz.cashguo.top/gtwnpiqccw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jyoumei.cn/gtegoyywkq.html

[R09] 字符串比较
来源：http://hz.sysykeji.top/gtjihxgibw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.snrcjt.cn/gtilzqavil.html

[R10] 正则匹配
来源：http://hz.ppjwa.cn/gtayumtfty.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.smart0.xyz/gtdajbtork.html

[R11] case 多分支
来源：http://hz.cqqwz.cn/gtphmtdlil.html

case "$1" in
来源：http://hz.zhongyouzk.top/gtgkiqomht.html

start) echo "启动" ;;
来源：http://hz.wangshuangyany.cn/gtcsyivziw.html

stop)  echo "停止" ;;
来源：http://hz.zycfv.cn/gtugbjppkz.html

*)     echo "未知命令" ;;
来源：http://hz.0kj1m.cn/gtkglkwfwu.html

esac
来源：http://hz.fzhhl.top/gttnyhlbrv.html

[R12] for 遍历文件
来源：http://hz.zycfv.cn/gtchdqnfvw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.c1oappe.top/gtnuqantgc.html

[R13] for 计数循环
来源：http://hz.pengpengdd.cyou/gtevqnfahg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.quarkkingdee.top/gtodigjirz.html

[R14] C 风格 for
来源：http://hz.c1oappe.top/gtufzlhkgg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yuanzhike.top/gtibvkipfr.html

[R15] while 逐行读文件
来源：http://hz.jianghu66.top/gtuqbexfbi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aibaodan.cn/gtrdseiuxy.html

[R16] until 等待条件
来源：http://hz.xinyue.icu/gtqicfpfug.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xinyue.icu/gtpjatdyku.html

[R17] 数组定义与取值
来源：http://hz.redwolf501.top/gtmgjexawk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ppjwa.cn/gtwogggczo.html

[R18] 遍历数组
来源：http://hz.wangdashe.top/gtswcryxhn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shzxlz.cn/gtalgzpcer.html

[R19] 数组长度
来源：http://hz.hnxiangtu.top/gtnbrqgske.html

echo "${#arr[@]}"
来源：http://hz.xylfe.cn/gtypjaebir.html

[R20] 关联数组（字典）
来源：http://hz.jyoumei.cn/gtyfylpfuk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.guowangkeji.top/gtdwvgaeqp.html

[R21] 字符串长度
来源：http://hz.yj20258888.top/gtfdxyfhmi.html

echo "${#s}"
来源：http://hz.yvedp.cn/gtdkpglhml.html

[R22] 截取子串
来源：http://hz.52xcode.cn/gtbtbvnmyb.html

echo "${s:0:5}"
来源：http://hz.svipenyu.cn/gtjgofbeir.html

[R23] 字符串替换
来源：http://hz.hfpthk.cn/gtolizbfet.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sweek.top/gttmevxwmc.html

[R24] 大小写转换
来源：http://hz.yvedp.cn/gtpnjpcdnc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.meibo888.top/gtmdsnlhna.html

[R25] 去后缀 / 去前缀
来源：http://hz.guowangkeji.top/gtlflxdnex.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yvedp.cn/gtdfykekjn.html

[R26] 命令替换
来源：http://hz.zhoulong.xyz/gthxicxjqs.html

now=$(date +%F); echo "$now"
来源：http://hz.feifeiyinyue.top/gtsvgrtbin.html

[R27] 算术展开
来源：http://hz.tian-w.cn/gtjdlokqgl.html

echo $((1 + 2 * 3))
来源：http://hz.zhijiandao.cn/gtekknuhuk.html

[R28] 浮点运算
来源：http://hz.zhengqikj.top/gtgfcdpkwq.html

echo "scale=2; 10/3" | bc
来源：http://hz.sxryk.cn/gtsviwzrtx.html

[R29] 定义函数
来源：http://hz.hywenlv.cn/gtfqcxpcal.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hfpthk.cn/gtexyjbviq.html

[R30] 函数返回状态码
来源：http://hz.birdmap.top/gtpznnznqo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shzxlz.cn/gtllrcnsiw.html

[R31] 局部变量
来源：http://hz.hywenlv.cn/gttuldlglb.html

f() { local x=1; echo "$x"; }
来源：http://hz.hammf.cn/gtftwpqsoy.html

[R32] 参数个数校验
来源：http://hz.tianlin.xyz/gtxampajny.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cucudq.cn/gtgkcdprwd.html

[R33] 捕获错误并提示行号
来源：http://hz.yueranfly.top/gtkqzoxelz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.aibaodan.cn/gtwpzoqjpp.html

[R34] 退出时清理
来源：http://hz.redwolf501.top/gtuikgrbnm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xziqi.cn/gtztdcybtv.html

[R35] 后台执行并等待
来源：http://hz.mhx1999.top/gtbykibxtx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinyuanbaomall.cn/gtbxgbutru.html

[R36] 并发执行多个任务
来源：http://hz.xuanzx.com/gtmryfwipn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nanxuanxn.top/gtpxdfewak.html

[R37] 把输出赋给变量
来源：http://hz.bjfxy.top/gtgvizbqxi.html

files=$(ls -1)
来源：http://hz.hnqzz.top/gtvgvxbgrc.html

[R38] 管道串联
来源：http://hz.wangdashe.top/gttlrfepwk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinghuilouyu.cn/gtwyxicpzg.html

[R39] 重定向标准输出与错误
来源：http://hz.tian-w.cn/gtvlfonkoh.html

cmd > out.log 2>&1
来源：http://hz.316326.xyz/gtxmhyyggr.html

[R40] 追加写日志
来源：http://hz.shanyushiyangkeji.top/gtbfytcdcu.html

echo "log" >> out.log
来源：http://hz.jinyuanbaomall.cn/gtruhfhujv.html

[R41] 丢弃输出
来源：http://hz.xylfe.cn/gtnvcnaufy.html

cmd >/dev/null 2>&1
来源：http://hz.hongshengwenyu.top/gtkqrrugzi.html

[R42] 输入重定向
来源：http://hz.yj20258888.top/gtglyacuhb.html

wc -l < a.txt
来源：http://hz.zdqjudy.top/gtghcvowhg.html

[R43] 按名字查找文件
来源：http://hz.jqgfzy.top/gtilllhoso.html

find . -name "*.log" -type f
来源：http://hz.mhx1999.top/gtholzdzew.html

[R44] 按修改时间查找
来源：http://hz.yanxiufei.cn/gtmwzdyffo.html

find . -mtime -7 -type f
来源：http://hz.cdnleiting.top/gtydusjjyg.html

[R45] 批量删除
来源：http://hz.meibo888.top/gtzsukecfd.html

find . -name "*.tmp" -delete
来源：http://hz.sxryk.cn/gtssrgoxmk.html

[R46] 递归替换文件内容
来源：http://hz.vqdsnc.cn/gtolosffpb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jianghu66.top/gtsngyjaxi.html

[R47] sed 单行替换
来源：http://hz.kuanghao11.cn/gtuoxrjggd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.tian-w.cn/gtdggzffsw.html

[R48] awk 取指定列
来源：http://hz.ehwqpu.com/gtsylttgrg.html

awk '{print $1, $3}' a.txt
来源：http://hz.tanke756.top/gtrdmqjscp.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gtkhkynvwy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shzxlz.cn/gtenbvstru.html

[R50] awk 求和
来源：http://hz.jinqigfzy.top/gtyfhbrilh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hammf.cn/gtilwizlck.html

[R51] 排序去重取前几
来源：http://hz.yonumen.top/gtfjddjiwg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yuxming.cn/gtkfetaeaz.html

[R52] 统计行数
来源：http://hz.ybcxt.top/gtbitzklwh.html

wc -l a.txt
来源：http://hz.yj202588.top/gtjomxvjgz.html

[R53] 查看文件头与实时尾
来源：http://hz.ehwqpu.com/gtsyenpihq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yueranfly.top/gtsolqiylp.html

[R54] 比较两个文件
来源：http://hz.aizwys.cn/gtbdqodtht.html

diff a.txt b.txt
来源：http://hz.chenjidiqi.icu/gtsxmwqjok.html

[R55] 压缩与解压
来源：http://hz.yj20258.top/gtwmxbnezz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yueranfly.top/gtmxemofnm.html

[R56] 远程拷贝
来源：http://hz.svipenyu.cn/gtcwnirdtp.html

scp file user@host:/path/
来源：http://hz.guowangkeji.top/gthpxgalca.html

[R57] 远程执行命令
来源：http://hz.jiagoushi.top/gtkmnundgk.html

ssh user@host 'uptime'
来源：http://hz.dianchejie.cn/gtoesezkxt.html

[R58] 下载文件
来源：http://hz.zhixingplan.top/gtpyevlefi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.bjfxy.top/gtesqwuksh.html

[R59] 发 POST JSON
来源：http://hz.xuanzx.com/gtllplzahy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yangfankeji.com/gtviywgntn.html

[R60] 只看 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtvgyvipkk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jlsjyb.cn/gtkgxzvsvb.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gtrsbzzafd.html

df -h;  du -sh *
来源：http://hz.nwbrower.top/gtaaagsclr.html

[R62] 找最占空间的文件
来源：http://hz.havefunace.top/gtundrevet.html

du -ah . | sort -rh | head -10
来源：http://hz.yanxiufei.cn/gtabnzggzy.html

[R63] 内存与进程
来源：http://hz.zycfv.cn/gtqkhiqcfj.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxinkj.top/gtodbvnwve.html

[R64] 结束进程
来源：http://hz.sxryk.cn/gtypuxgnfo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.bjfxy.top/gtlnfczqbh.html

[R65] 查看端口占用
来源：http://hz.xinyue.icu/gtgijkstws.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zycfv.cn/gtxyxfphed.html

[R66] 定时任务
来源：http://hz.quarkkingdee.top/gttsswmhyf.html

crontab -e;  crontab -l
来源：http://hz.jyoumei.cn/gtzgmxkxgj.html

[R67] 生成随机十六进制串
来源：http://hz.guannengcc.top/gtozythkmt.html

openssl rand -hex 16
来源：http://hz.sxryk.cn/gterxvmgij.html

[R68] 计算文件校验值
来源：http://hz.cucudq.cn/gtomrgextt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cheryme.top/gtldygkwaw.html

[R69] 生成随机密码
来源：http://hz.yuanzhike.top/gtwsmrwhqv.html

head -c 16 /dev/urandom | base64
来源：http://hz.hnxiangtu.top/gtsvdbasuy.html

[R70] 时间戳与互转
来源：http://hz.chenzaomai.com/gtlvcpmwck.html

date +%s;  date -d @1700000000
来源：http://hz.cqqwz.cn/gtihogiduj.html

[R71] 日期格式化
来源：http://hz.zhixingplan.top/gtfmwxcwvr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj20258888.top/gttdlrosnm.html

[R72] 等待端口就绪
来源：http://hz.feifeiyinyue.top/gthxffuyfr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hywenlv.cn/gtolvuldqq.html

[R73] 分割大日志
来源：http://hz.tianlin.xyz/gthasbobqz.html

split -l 1000 big.log part_
来源：http://hz.iojbl.cn/gttnkwdewg.html

[R74] 批量重命名
来源：http://hz.9152youxi.cn/gtibewqkye.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yanxiufei.cn/gtnirnyzmu.html

[R75] 导出环境变量
来源：http://hz.redwolf501.top/gtbpnaiwei.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shanyushiyangtech.top/gtwvhtevww.html

[R76] 使用临时文件
来源：http://hz.shzxlz.cn/gtvbdhplwl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dashuyun.cn/gthywqbarx.html

[R77] 读取用户输入
来源：http://hz.0kj1m.cn/gtdmaaddmk.html

read -rp "请输入: " ans
来源：http://hz.shanyushiyangtech.top/gtqavsklos.html

[R78] 交互式菜单
来源：http://hz.bjfxy.top/gtqkzmdbfc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.snrcjt.cn/gtqxohbjsm.html

[R79] 解析命令行选项
来源：http://hz.jinyuanbaomall.cn/gtnnklvmjv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daria6918.cn/gtsgclfrmg.html

[R80] 查看脚本执行耗时
来源：http://hz.chenjidiqi.icu/gtwnnbsjkq.html

time ./run.sh
来源：http://hz.daria6918.cn/gtameknhcz.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtfevdfimt.html

S. C / C++ 专题
来源：http://hz.hywenlv.cn/gtrlrlngew.html

================================================================================
来源：http://hz.andypj.xyz/gtwemsxgkj.html

[S01] C：Hello World
来源：http://hz.daxiang520.top/gtayoddccj.html

#include <stdio.h>
来源：http://hz.jqgfzy.top/gtzzmtjlgm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hongshengwenyu.top/gtnhblrdos.html

[S02] C：变量与格式化输出
来源：http://hz.zycfv.cn/gtugyjziqe.html

int a = 10; printf("%d\n", a);
来源：http://hz.tanke756.top/gtkslvnajn.html

[S03] C：读入整数
来源：http://hz.zycfv.cn/gtbqlazxen.html

int x; scanf("%d", &x);
来源：http://hz.svipenyu.cn/gtzkiuhumd.html

[S04] C：字符串复制
来源：http://hz.jyoumei.cn/gtmxmpuihc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xingfuxueyuan.xyz/gtthvvgcyg.html

[S05] C：字符串长度
来源：http://hz.zhongyouzk.top/gtwricmjlf.html

strlen(s)
来源：http://hz.jqgfzy.top/gtatqmbqus.html

[S06] C：字符串比较
来源：http://hz.dashuyun.cn/gttvicbldg.html

strcmp(a, b) == 0
来源：http://hz.xuetiantiany.cn/gtlpnvbipc.html

[S07] C：数组遍历求和
来源：http://hz.zhengqikj.top/gtfqbgohrk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.bjfxy.top/gtudonvlmg.html

[S08] C：动态内存分配与释放
来源：http://hz.quarkkingdee.top/gtqowpxszl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yongpay.top/gttltshvyv.html

[S09] C：结构体定义与初始化
来源：http://hz.xuetiantiany.cn/gtaixwuwsr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xuetiantiany.cn/gtijztgfmi.html

[S10] C：指针与解引用
来源：http://hz.gogol.net.cn/gtnxobdejc.html

int *p = &a;  *p = 5;
来源：http://hz.yueranfly.top/gtvpwtrlkj.html

[S11] C：逐行读文件
来源：http://hz.jinqigfzy.top/gtuetljkto.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jiagoushi.top/gthlztmkzx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.52xcode.cn/gthwxpjkqb.html

fclose(f);
来源：http://hz.jyoumei.cn/gtfoixhbsj.html

[S12] C：写文件
来源：http://hz.guannengcc.top/gtcjzescyf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shanyushiyangtech.top/gttmwolxny.html

[S13] C：宏定义
来源：http://hz.0kj1m.cn/gtzxvlueac.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.andypj.xyz/gteetvodcm.html

[S14] C：枚举
来源：http://hz.hfpthk.cn/gtbbtjczcu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.guannengcc.top/gtzsmkvznr.html

[S15] C：类型转换
来源：http://hz.fengsongda.top/gtgrheayrf.html

(double) a / b
来源：http://hz.52xcode.cn/gtkrkgjdor.html

[S16] C：位操作置位
来源：http://hz.cdnleiting.top/gthjczxcbx.html

x |= (1 << 3);
来源：http://hz.jinqigfzy.top/gtoguqdmlc.html

[S17] C：安全拼接字符串
来源：http://hz.haohaochexian.top/gtkehhgwfz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ywan-chungtsiang.top/gtupntulfr.html

[S18] C：命令行参数
来源：http://hz.9152youxi.cn/gtznzsrzab.html

int main(int argc, char **argv)
来源：http://hz.yanxiufei.cn/gtfbepvqru.html

[S19] C：快速排序
来源：http://hz.sufxvd.cn/gtnoqgizfh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.feifeiyinyue.top/gtmixdoqtc.html

[S20] C：二分查找
来源：http://hz.jlsjyb.cn/gtxglijdcu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.wangdashe.top/gtkfgkasxe.html

[S21] C：字符类别判断
来源：http://hz.gotoacloud.top/gtkuepgamm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.redwolf501.top/gtejiorkwb.html

[S22] C：字符串转数字
来源：http://hz.quarkkingdee.top/gtbdkjuhoe.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.wangdashe.top/gtwpwaajwv.html

[S23] C：随机数
来源：http://hz.cdnleiting.top/gtqooyhdra.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yuanzhike.top/gtvkunptem.html

[S24] C：获取本地时间
来源：http://hz.pengpengdd.cyou/gtkljdhsjc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangdashe.top/gtgcstzwti.html

[S25] C：内存拷贝
来源：http://hz.xinyue.icu/gteecdpezr.html

memcpy(dst, src, n);
来源：http://hz.cdnleiting.top/gtuprgdmpc.html

[S26] C：内存清零
来源：http://hz.fzhhl.top/gtbshexgsy.html

memset(a, 0, sizeof a);
来源：http://hz.vqdsnc.cn/gtpsdtvavm.html

[S27] C：定义常量
来源：http://hz.tian-w.cn/gtgmoypndk.html

const double PI = 3.14159;
来源：http://hz.guowangkeji.top/gtxusvtbfh.html

[S28] C：静态变量
来源：http://hz.zhoulong.xyz/gtfsyqsuxc.html

static int counter = 0;
来源：http://hz.nanxuanxn.top/gtuzmzktde.html

[S29] C：变参函数
来源：http://hz.cucudq.cn/gtgihfjglq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hongshengwenyu.top/gtegtegfht.html

[S30] C：头文件保护
来源：http://hz.yj20258.top/gthhqlqjul.html

#ifndef X_H
来源：http://hz.xuetiantiany.cn/gtwxwgvkry.html

#define X_H
来源：http://hz.xingfuxueyuan.xyz/gtsmnktfls.html

#endif
来源：http://hz.yongpay.top/gttypgpcvq.html

[S31] C++：Hello World
来源：http://hz.chenzaomai.com/gtwxewkmzt.html

#include <iostream>
来源：http://hz.nwbrower.top/gtjjvlqmvv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenjidiqi.icu/gtfhbtxshu.html

[S32] C++：字符串
来源：http://hz.hywenlv.cn/gteumygbmk.html

std::string s = "hi";  s += "!";
来源：http://hz.shzxlz.cn/gtdtjuivqa.html

[S33] C++：vector 增删
来源：http://hz.hnqzz.top/gtoqjegvfl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tianlin.xyz/gtpgpoowli.html

[S34] C++：遍历 vector
来源：http://hz.yangfankeji.com/gttknklace.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fengsongda.top/gtiwwqqezy.html

[S35] C++：map
来源：http://hz.cashguo.top/gtmflwgfin.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtrbtharmm.html

[S36] C++：unordered_map
来源：http://hz.hywenlv.cn/gtlhljqokv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhongyouzk.top/gtlbsyyzyx.html

[S37] C++：set
来源：http://hz.quarkkingdee.top/gtckpbqyyf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.kuanghao11.cn/gthkfetice.html

[S38] C++：排序
来源：http://hz.zhoulong.xyz/gtdjsxdhxw.html

std::sort(v.begin(), v.end());
来源：http://hz.kuanghao11.cn/gtynekuitb.html


<!-- 参考信息 -->