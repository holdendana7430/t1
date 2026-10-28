代发 wailian999

ROLLBACK TO sp1;
来源：http://hz.ydjk.org.cn/gtouzjqqnw.html

[Q69] 查看执行计划
来源：http://hz.yj202588.top/gtvmmexiah.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ydjk.org.cn/gtxjfmwddg.html

[Q70] 更新统计信息
来源：http://hz.yvedp.cn/gtiyejxrsa.html

ANALYZE TABLE users;
来源：http://hz.zdqjudy.top/gtprxcylkd.html

[Q71] 查看建表语句
来源：http://hz.sweek.top/gtozhsicap.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.redwolf501.top/gtefracfyf.html

[Q72] 查看索引
来源：http://hz.cucudq.cn/gtpjokxhgt.html

SHOW INDEX FROM users;
来源：http://hz.tian-w.cn/gtojiwblzs.html

[Q73] 查看表状态
来源：http://hz.cqqwz.cn/gtxnfpzkna.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.mhx1999.top/gtxcaxbhgr.html

[Q74] 强制使用索引
来源：http://hz.guannengcc.top/gtnoanwbvb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenlongwang.top/gtsqefmjbd.html

[Q75] 日期格式化
来源：http://hz.xinyue.icu/gtejcfnutk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ppjwa.cn/gtfxigsfsy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xingfuxueyuan.xyz/gtvwkxwvar.html

[Q76] 按天统计
来源：http://hz.jinyuanbaomall.cn/gtqvaqztjq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nwbrower.top/gttviqxwqh.html

[Q77] 时间加减
来源：http://hz.sysykeji.top/gtdowdwrxi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gogol.net.cn/gtbmzdvwlv.html

[Q78] 当前时间
来源：http://hz.hnqzz.top/gtaotloipu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hywenlv.cn/gtsrsndyea.html

[Q79] 字符串拼接
来源：http://hz.gzhubu.top/gtuhjuckdc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.feifeiyinyue.top/gtrwniovil.html

[Q80] 字符串截取
来源：http://hz.kuanghao11.cn/gtfndbhgrk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhengqikj.top/gtdpyhiban.html

[Q81] 字符串替换
来源：http://hz.jinqigfzy.top/gtgrifmhes.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hfpthk.cn/gtgpckdzag.html

[Q82] 字符长度与字节长度
来源：http://hz.hywenlv.cn/gtmyqgmqqn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhijiandao.cn/gtyxekxiwu.html

[Q83] 大小写转换
来源：http://hz.yangfankeji.com/gtclqheowc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.chenlongwang.top/gthwmiiagg.html

[Q84] 去除首尾空格
来源：http://hz.meibo888.top/gtlmjyhgxs.html

SELECT TRIM(name) FROM users;
来源：http://hz.zdqjudy.top/gteanujdts.html

[Q85] 数值取整
来源：http://hz.jinqigfzy.top/gtsunawkgz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tanke756.top/gtnzqjprsr.html

[Q86] 读取 JSON 字段
来源：http://hz.smart0.xyz/gtamaygzsh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.aibaodan.cn/gtvdocjhut.html

[Q87] JSON 字段做条件
来源：http://hz.316326.xyz/gtlbpwthvr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhijiandao.cn/gtcaaratqq.html

[Q88] 行转列（条件聚合）
来源：http://hz.yvedp.cn/gtqxewnfey.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gtnetbyhta.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hfpthk.cn/gtepmojpfj.html

[Q89] 判断表是否存在
来源：http://hz.chenzaomai.com/gtwtaozjhm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cdnleiting.top/gtsofggeft.html

[Q90] 生成序号列
来源：http://hz.chenjidiqi.icu/gtkuqaviws.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ivvv.top/gtkdyhuise.html

================================================================================
来源：http://hz.hywenlv.cn/gtkpoykdef.html

R. Bash 专题
来源：http://hz.aibaodan.cn/gtvjlbnmdx.html

================================================================================
来源：http://hz.jlsjyb.cn/gtoidxfyfi.html

[R01] shebang 与严格模式
来源：http://hz.hammf.cn/gtligiuxda.html

#!/usr/bin/env bash
来源：http://hz.jqgfzy.top/gtbwkulkui.html

set -euo pipefail
来源：http://hz.jiagoushi.top/gtshxqncja.html

[R02] 变量赋值与使用
来源：http://hz.yongpay.top/gtvkxvfmcx.html

name="Tom"; echo "$name"
来源：http://hz.zdqjudy.top/gtghkqlmmb.html

[R03] 只读变量
来源：http://hz.jianghu66.top/gtqrgsgyhc.html

readonly PI=3.14
来源：http://hz.jinghuilouyu.cn/gtsjvwcvkr.html

[R04] 位置参数
来源：http://hz.jqgfzy.top/gtzhahyunj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.9152youxi.cn/gtkoxumcfj.html

[R05] 参数默认值
来源：http://hz.xuanzx.com/gtkicdwaxl.html

name="${1:-default}"
来源：http://hz.jqgfzy.top/gtxmoucaaz.html

[R06] 判断命令是否存在
来源：http://hz.zhongyouzk.top/gtswdeovny.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258888.top/gtnfcswkgu.html

[R07] if 判断文件
来源：http://hz.daria6918.cn/gtmgipcqjh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tian-w.cn/gtfpgnvnvu.html

[R08] 数值比较
来源：http://hz.ywan-chungtsiang.top/gtwxqjslqf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangshuangyany.cn/gtmweqnhzb.html

[R09] 字符串比较
来源：http://hz.cqqwz.cn/gtxekzwzlh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ybcxt.top/gtxjkadyth.html

[R10] 正则匹配
来源：http://hz.birdmap.top/gtazrinwda.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sysykeji.top/gtijbjtitl.html

[R11] case 多分支
来源：http://hz.pengpengdd.cyou/gtmxojlrrb.html

case "$1" in
来源：http://hz.jyoumei.cn/gtkuanumct.html

start) echo "启动" ;;
来源：http://hz.yuxming.cn/gtvscdfxno.html

stop)  echo "停止" ;;
来源：http://hz.zhengqikj.top/gtnhbqkuut.html

*)     echo "未知命令" ;;
来源：http://hz.aibaodan.cn/gtvwtqkpsl.html

esac
来源：http://hz.cucudq.cn/gttybzoowx.html

[R12] for 遍历文件
来源：http://hz.sweek.top/gtphxmcvpt.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ivvv.top/gtwedhwmlm.html

[R13] for 计数循环
来源：http://hz.xuanzx.com/gtwdojucdw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shanyushiyangtech.top/gttqkweizm.html

[R14] C 风格 for
来源：http://hz.jianghu66.top/gtusvxvgnm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jyoumei.cn/gtemccjjpj.html

[R15] while 逐行读文件
来源：http://hz.bjfxy.top/gtpibtfyhn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.andypj.xyz/gtdpwkyxwo.html

[R16] until 等待条件
来源：http://hz.redwolf501.top/gttbbmmhub.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtvhlssimr.html

[R17] 数组定义与取值
来源：http://hz.smart0.xyz/gtpiamzdds.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydzc1.top/gtvddtvalu.html

[R18] 遍历数组
来源：http://hz.shuidangran.top/gttsblzbxq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sysykeji.top/gthguewlri.html

[R19] 数组长度
来源：http://hz.hysaishi.cn/gthggvwkhe.html

echo "${#arr[@]}"
来源：http://hz.daxiang520.top/gtldyhcoft.html

[R20] 关联数组（字典）
来源：http://hz.jiagoushi.top/gtyticlemk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangkeji.top/gtsynifktr.html

[R21] 字符串长度
来源：http://hz.hfpthk.cn/gtssnlmaum.html

echo "${#s}"
来源：http://hz.jinqigufen.top/gtxlzrmzln.html

[R22] 截取子串
来源：http://hz.jlsjyb.cn/gtcqrnvlyr.html

echo "${s:0:5}"
来源：http://hz.snrcjt.cn/gtfrwydeua.html

[R23] 字符串替换
来源：http://hz.jinqigfzy.top/gtbdyttwae.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.316326.xyz/gtcyogajnk.html

[R24] 大小写转换
来源：http://hz.nanxuanxn.top/gtamnfyfuo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258888.top/gtxqwmodqq.html

[R25] 去后缀 / 去前缀
来源：http://hz.gaohongyu789.top/gtknujpsyt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.52xcode.cn/gtjttbzmwy.html

[R26] 命令替换
来源：http://hz.zhengqikj.top/gtuuyzqbio.html

now=$(date +%F); echo "$now"
来源：http://hz.yanxiufei.cn/gtshwubjii.html

[R27] 算术展开
来源：http://hz.dianchejie.cn/gtbhvfacrc.html

echo $((1 + 2 * 3))
来源：http://hz.hywenlv.cn/gtqszmavno.html

[R28] 浮点运算
来源：http://hz.9152youxi.cn/gtgfjsjnaf.html

echo "scale=2; 10/3" | bc
来源：http://hz.cashguo.top/gtxlffhjxk.html

[R29] 定义函数
来源：http://hz.fengsongda.top/gtdzivkgdw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jianghu66.top/gtgirmolrk.html

[R30] 函数返回状态码
来源：http://hz.ydjk.org.cn/gtllihgnhu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hammf.cn/gtysvdsnqn.html

[R31] 局部变量
来源：http://hz.gotoacloud.top/gtjhudlkbb.html

f() { local x=1; echo "$x"; }
来源：http://hz.sysykeji.top/gtqgqwguqp.html

[R32] 参数个数校验
来源：http://hz.zhoulong.xyz/gtqgggyojs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gtizixrgsp.html

[R33] 捕获错误并提示行号
来源：http://hz.kuanghao11.cn/gtetbrjvvl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigfzy.top/gtujhsclpp.html

[R34] 退出时清理
来源：http://hz.ydzc1.top/gtcxrkokuc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cashguo.top/gtdbmhbppd.html

[R35] 后台执行并等待
来源：http://hz.zdqjudy.top/gtyylomuew.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.fzhhl.top/gtnjrmdeuc.html

[R36] 并发执行多个任务
来源：http://hz.guowangkeji.top/gtqkzitsdg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinqigfzy.top/gtswttogvb.html

[R37] 把输出赋给变量
来源：http://hz.52xcode.cn/gtopsquzve.html

files=$(ls -1)
来源：http://hz.chenjidiqi.icu/gtaimdryms.html

[R38] 管道串联
来源：http://hz.ydzc1.top/gtbikindrc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinqigufen.top/gtsiruhorc.html

[R39] 重定向标准输出与错误
来源：http://hz.tanke756.top/gthjaygtih.html

cmd > out.log 2>&1
来源：http://hz.zhongyouzk.top/gtustaaokv.html

[R40] 追加写日志
来源：http://hz.mhx1999.top/gtaquuvrel.html

echo "log" >> out.log
来源：http://hz.nwbrower.top/gtrhzkiize.html

[R41] 丢弃输出
来源：http://hz.cqqwz.cn/gtrjpjfzeb.html

cmd >/dev/null 2>&1
来源：http://hz.xziqi.cn/gtpjyywktm.html

[R42] 输入重定向
来源：http://hz.hammf.cn/gtvxomarpq.html

wc -l < a.txt
来源：http://hz.xuanzx.com/gtlxvodtqp.html

[R43] 按名字查找文件
来源：http://hz.shangyingyoupin.top/gtsxqhvrnk.html

find . -name "*.log" -type f
来源：http://hz.zhengqikj.top/gtopoopchx.html

[R44] 按修改时间查找
来源：http://hz.yongpay.top/gtedbbvmic.html

find . -mtime -7 -type f
来源：http://hz.cucudq.cn/gtzhrhjyca.html

[R45] 批量删除
来源：http://hz.52xcode.cn/gtpagcwtkb.html

find . -name "*.tmp" -delete
来源：http://hz.jinqigfzy.top/gtxdjsbplp.html

[R46] 递归替换文件内容
来源：http://hz.feifeiyinyue.top/gtdnhymuzw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sxryk.cn/gtruzpzjaq.html

[R47] sed 单行替换
来源：http://hz.9152youxi.cn/gtagtalqqj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jqgufenzy.top/gtxmcrckwx.html

[R48] awk 取指定列
来源：http://hz.sweek.top/gtjlhsrcfw.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhixingplan.top/gtucatnixo.html

[R49] awk 带条件
来源：http://hz.birdmap.top/gtonmhpmpl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hongshengwenyu.top/gtolpxijwd.html

[R50] awk 求和
来源：http://hz.bjfxy.top/gttawryxuj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258888.top/gtujdjjvlq.html

[R51] 排序去重取前几
来源：http://hz.aizwys.cn/gtdkfhzgid.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cashguo.top/gtkyvctfmh.html

[R52] 统计行数
来源：http://hz.xziqi.cn/gtgljnuslp.html

wc -l a.txt
来源：http://hz.xingfuxueyuan.xyz/gtvhqwjpry.html

[R53] 查看文件头与实时尾
来源：http://hz.yj202588.top/gttecimejk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.feifeiyinyue.top/gtsjiixmbd.html

[R54] 比较两个文件
来源：http://hz.tanke756.top/gtbbynvhpj.html

diff a.txt b.txt
来源：http://hz.daria6918.cn/gtixxqmmhg.html

[R55] 压缩与解压
来源：http://hz.cucudq.cn/gtqyaxaihi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sxryk.cn/gtjiacawps.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangkeji.top/gtkttalrdj.html

scp file user@host:/path/
来源：http://hz.guannengcc.top/gtnblyyquc.html

[R57] 远程执行命令
来源：http://hz.andypj.xyz/gtszqkxtdu.html

ssh user@host 'uptime'
来源：http://hz.hysaishi.cn/gtjvhkybbc.html

[R58] 下载文件
来源：http://hz.iojbl.cn/gtgtsdmhcm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ywan-chungtsiang.top/gtlwpcspay.html

[R59] 发 POST JSON
来源：http://hz.ppjwa.cn/gtvnlhmfyu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.redwolf501.top/gtkyqmnrkx.html

[R60] 只看 HTTP 状态码
来源：http://hz.ivvv.top/gtpubaqiud.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinyuanbaomall.cn/gtixaingkq.html

[R61] 磁盘占用
来源：http://hz.fengsongda.top/gtckkmeajc.html

df -h;  du -sh *
来源：http://hz.kuanghao11.cn/gtocwrgcdm.html

[R62] 找最占空间的文件
来源：http://hz.daxiang520.top/gtmdtlfwin.html

du -ah . | sort -rh | head -10
来源：http://hz.svipenyu.cn/gtxotjawta.html

[R63] 内存与进程
来源：http://hz.9152youxi.cn/gtccrmsexe.html

free -h;  ps aux | grep nginx
来源：http://hz.pengpengdd.cyou/gtneklkxgq.html

[R64] 结束进程
来源：http://hz.cdnleiting.top/gtmckqkryq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nwbrower.top/gtgrnwkihh.html

[R65] 查看端口占用
来源：http://hz.jianghu66.top/gtjiueqosi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yongpay.top/gtbmltkuml.html

[R66] 定时任务
来源：http://hz.shzxlz.cn/gtvfdkwmqy.html

crontab -e;  crontab -l
来源：http://hz.nwbrower.top/gtrufvkzph.html

[R67] 生成随机十六进制串
来源：http://hz.xinyue.icu/gtsmohcbma.html

openssl rand -hex 16
来源：http://hz.zhaomingkeji.xyz/gtpqftsgii.html

[R68] 计算文件校验值
来源：http://hz.cheryme.top/gterpmkwis.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sysykeji.top/gtukvjprtn.html

[R69] 生成随机密码
来源：http://hz.jyoumei.cn/gtzzszelwq.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenjidiqi.icu/gtgabezomy.html

[R70] 时间戳与互转
来源：http://hz.nanxinkj.top/gtkohqrgqz.html

date +%s;  date -d @1700000000
来源：http://hz.xingfuxueyuan.xyz/gtdbfxuvxr.html

[R71] 日期格式化
来源：http://hz.aizwys.cn/gtzbzlihko.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yongpay.top/gtujjpiudl.html

[R72] 等待端口就绪
来源：http://hz.havefunace.top/gtgshiqldm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shzxlz.cn/gtpqxqoxol.html

[R73] 分割大日志
来源：http://hz.daxiang520.top/gtscyjusfm.html

split -l 1000 big.log part_
来源：http://hz.316326.xyz/gtlcgnzdep.html

[R74] 批量重命名
来源：http://hz.haohaochexian.top/gtkjhlqwsx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.bjfxy.top/gtuzjyfivh.html

[R75] 导出环境变量
来源：http://hz.ybcxt.top/gtkialvjdb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhoulong.xyz/gtijmpuzco.html

[R76] 使用临时文件
来源：http://hz.sxryk.cn/gtslujxeuy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.guannengcc.top/gtgxhbxjaw.html

[R77] 读取用户输入
来源：http://hz.dianchejie.cn/gtpbdljgow.html

read -rp "请输入: " ans
来源：http://hz.jinghuilouyu.cn/gtbfgseztd.html

[R78] 交互式菜单
来源：http://hz.ydzc1.top/gtdhangnqu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.meibo888.top/gtiubufdha.html

[R79] 解析命令行选项
来源：http://hz.svipenyu.cn/gtevudvhux.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.andypj.xyz/gttzfdmwmr.html

[R80] 查看脚本执行耗时
来源：http://hz.sufxvd.cn/gtnykgcfbv.html

time ./run.sh
来源：http://hz.xinyue.icu/gtngibocxl.html

================================================================================
来源：http://hz.cashguo.top/gtfgtsztxy.html

S. C / C++ 专题
来源：http://hz.feifeiyinyue.top/gtmfislkfz.html

================================================================================
来源：http://hz.52xcode.cn/gtypgapxbf.html

[S01] C：Hello World
来源：http://hz.yuxming.cn/gttqveixxr.html

#include <stdio.h>
来源：http://hz.yanxiufei.cn/gtyrholqrh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ywan-chungtsiang.top/gtdefnwoos.html

[S02] C：变量与格式化输出
来源：http://hz.jyoumei.cn/gtoesxchbl.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuanzhike.top/gtwgnzfgxx.html

[S03] C：读入整数
来源：http://hz.52xcode.cn/gtpwcesxun.html

int x; scanf("%d", &x);
来源：http://hz.aizwys.cn/gtjtmlciyh.html

[S04] C：字符串复制
来源：http://hz.chenjidiqi.icu/gtaafgaqim.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.aibaodan.cn/gtiazterqv.html

[S05] C：字符串长度
来源：http://hz.snrcjt.cn/gtiqrnokoj.html

strlen(s)
来源：http://hz.iojbl.cn/gtlhxhtxqb.html

[S06] C：字符串比较
来源：http://hz.daria6918.cn/gtashofdha.html

strcmp(a, b) == 0
来源：http://hz.ppjwa.cn/gtsztuwevk.html

[S07] C：数组遍历求和
来源：http://hz.zhixingplan.top/gtbeytahru.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhongyouzk.top/gtqztlmgkk.html

[S08] C：动态内存分配与释放
来源：http://hz.cucudq.cn/gtesvlhjxm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nanxuanxn.top/gthhiqsteu.html

[S09] C：结构体定义与初始化
来源：http://hz.hammf.cn/gtsmhsxsfe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ydzc1.top/gtmjnxfxgs.html

[S10] C：指针与解引用
来源：http://hz.fengsongda.top/gtxzurjdxl.html

int *p = &a;  *p = 5;
来源：http://hz.shangyingyoupin.top/gtlbkjekwr.html

[S11] C：逐行读文件
来源：http://hz.tian-w.cn/gtakuhyjgk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.birdmap.top/gtksekxqgf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shzxlz.cn/gtkjgcocjw.html

fclose(f);
来源：http://hz.yvedp.cn/gthgqlfpgo.html

[S12] C：写文件
来源：http://hz.andypj.xyz/gtlchjhypx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tian-w.cn/gtyivgxirw.html

[S13] C：宏定义
来源：http://hz.ywan-chungtsiang.top/gtclxgchva.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shuidangran.top/gtbijwjdjq.html

[S14] C：枚举
来源：http://hz.hnqzz.top/gthhowmcmd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.haohaochexian.top/gtnaxsdekb.html

[S15] C：类型转换
来源：http://hz.yongpay.top/gttuucjuhu.html

(double) a / b
来源：http://hz.meibo888.top/gtosjjisgi.html

[S16] C：位操作置位
来源：http://hz.hnxiangtu.top/gtqaseukwf.html

x |= (1 << 3);
来源：http://hz.redwolf501.top/gtfhknvsba.html

[S17] C：安全拼接字符串
来源：http://hz.daxiang520.top/gtpqvvvuyd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hammf.cn/gtysinpyce.html

[S18] C：命令行参数
来源：http://hz.dashuyun.cn/gtuiotmzht.html

int main(int argc, char **argv)
来源：http://hz.shuidangran.top/gtnmdlkzai.html

[S19] C：快速排序
来源：http://hz.jiagoushi.top/gtnksgtlyt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtpubtmbhe.html

[S20] C：二分查找
来源：http://hz.jlsjyb.cn/gtbcbdcnda.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.bjfxy.top/gtmyqqnwoy.html

[S21] C：字符类别判断
来源：http://hz.daria6918.cn/gtihtikblh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ehwqpu.com/gtfqcureyg.html

[S22] C：字符串转数字
来源：http://hz.haohaochexian.top/gtzwsrkqee.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.havefunace.top/gtfaminqpk.html

[S23] C：随机数
来源：http://hz.sysykeji.top/gtnxngpiou.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xinyue.icu/gtuxrepbxi.html

[S24] C：获取本地时间
来源：http://hz.jyoumei.cn/gtlbrijxzw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.pengpengdd.cyou/gtifhbhotx.html

[S25] C：内存拷贝
来源：http://hz.xuanzx.com/gtvtgtkxwr.html

memcpy(dst, src, n);
来源：http://hz.redwolf501.top/gtiflfvsnf.html

[S26] C：内存清零
来源：http://hz.yongpay.top/gthnltiqyp.html

memset(a, 0, sizeof a);
来源：http://hz.cucudq.cn/gtoxfbnakf.html

[S27] C：定义常量
来源：http://hz.ybcxt.top/gtomtmzwjr.html

const double PI = 3.14159;
来源：http://hz.andypj.xyz/gtnkytcfgx.html

[S28] C：静态变量
来源：http://hz.yj20258.top/gtikafbmky.html

static int counter = 0;
来源：http://hz.nanxinkj.top/gtrrdzlblf.html

[S29] C：变参函数
来源：http://hz.zhaomingkeji.xyz/gttxqawldf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.kuanghao11.cn/gttrgpmajr.html

[S30] C：头文件保护
来源：http://hz.yongpay.top/gtjriplxlv.html

#ifndef X_H
来源：http://hz.sysykeji.top/gtmnurxyto.html

#define X_H
来源：http://hz.zhiwuduotai.top/gtzsplxmru.html

#endif
来源：http://hz.zdqjudy.top/gtkoeccwlk.html

[S31] C++：Hello World
来源：http://hz.mhx1999.top/gtswqchxau.html

#include <iostream>
来源：http://hz.andypj.xyz/gtxcjqjtzo.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.guannengcc.top/gtqqxfeixg.html

[S32] C++：字符串
来源：http://hz.shanyushiyangkeji.top/gttuyhswwx.html

std::string s = "hi";  s += "!";
来源：http://hz.shangyingyoupin.top/gtveziptpr.html

[S33] C++：vector 增删
来源：http://hz.xylfe.cn/gtwfulcmsn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.iojbl.cn/gtapxddccf.html

[S34] C++：遍历 vector
来源：http://hz.zycfv.cn/gtlvfbfrzh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.nanxuanxn.top/gtunsiwnfb.html

[S35] C++：map
来源：http://hz.chenjidiqi.icu/gtduyfhnyc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gtbxjxqfbq.html

[S36] C++：unordered_map
来源：http://hz.zycfv.cn/gtttaasiti.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hysaishi.cn/gttqokhiru.html

[S37] C++：set
来源：http://hz.hnqzz.top/gtebijgoac.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangtech.top/gtgekharqq.html

[S38] C++：排序
来源：http://hz.jinghuilouyu.cn/gtvajsabjm.html

std::sort(v.begin(), v.end());
来源：http://hz.sxryk.cn/gtcsaokcye.html


<!-- 参考信息 -->