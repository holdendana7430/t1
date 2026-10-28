代发 wailian999

[Q48] CTE 公用表表达式
来源：http://hz.shanyushiyangtech.top/gtqqxpeumu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shanyushiyangkeji.top/gtcpbqfrab.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cheryme.top/gtidybycce.html

[Q49] 更新单行
来源：http://hz.ybcxt.top/gtgdhfndsm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shangyingyoupin.top/gtcujzyadm.html

[Q50] 批量更新
来源：http://hz.shanyushiyangtech.top/gtgmbwzghd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xuetiantiany.cn/gtuuzntuxh.html

[Q51] 用子查询更新
来源：http://hz.cucudq.cn/gtefwtbckl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tanke756.top/gtmuiivabw.html

[Q52] 删除指定行
来源：http://hz.cheryme.top/gtysearduo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.birdmap.top/gthegjhadb.html

[Q53] 按条件删除
来源：http://hz.xingfuxueyuan.xyz/gtxnfcfoci.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shangyingyoupin.top/gtcviwukki.html

[Q54] 清空表
来源：http://hz.ybcxt.top/gtyvsdulfh.html

TRUNCATE TABLE logs;
来源：http://hz.daria6918.cn/gtjjbvgwcr.html

[Q55] 排名（并列占位）
来源：http://hz.daxiang520.top/gtuhflltsk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xziqi.cn/gtpvzxubnu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ehwqpu.com/gtqheepynb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhaomingkeji.xyz/gtjforycsx.html

[Q57] 行号
来源：http://hz.sufxvd.cn/gteeekoydh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.fengsongda.top/gtdzcstxib.html

[Q58] 累计求和
来源：http://hz.shanyushiyangtech.top/gtqitdtbsu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenjidiqi.icu/gtyqftnaix.html

[Q59] 分组内累计
来源：http://hz.yonumen.top/gtixagvrqo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigfzy.top/gttjkwiubo.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhaomingkeji.xyz/gtmbysjljz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.redwolf501.top/gtmctwljsu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.birdmap.top/gtazkbdoqn.html

[Q61] 移动平均
来源：http://hz.ehwqpu.com/gtvxvdcxuj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenlongwang.top/gtfgdxxdah.html

[Q62] 分组占比
来源：http://hz.xingfuxueyuan.xyz/gtflixooht.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtjuwpylmn.html

[Q63] 开启事务
来源：http://hz.smart0.xyz/gtxiveassm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenlongwang.top/gthyzbctce.html

[Q64] 提交事务
来源：http://hz.yvedp.cn/gtvrfcicoa.html

COMMIT;
来源：http://hz.zdqjudy.top/gtyptoncup.html

[Q65] 回滚事务
来源：http://hz.quarkkingdee.top/gtshobrfqo.html

ROLLBACK;
来源：http://hz.guannengcc.top/gtbusbshjl.html

[Q66] 行锁查询
来源：http://hz.pycfn.com/gtmfilnayk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinghuilouyu.cn/gtgubwiwki.html

[Q67] 设置隔离级别
来源：http://hz.cdnleiting.top/gtereeulbo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xylfe.cn/gtmbesqqcs.html

[Q68] 保存点
来源：http://hz.redwolf501.top/gtvbxwqmnh.html

SAVEPOINT sp1;
来源：http://hz.hongshengwenyu.top/gtpevaitot.html

ROLLBACK TO sp1;
来源：http://hz.fengsongda.top/gtnkvjfvnz.html

[Q69] 查看执行计划
来源：http://hz.ybcxt.top/gtduffpogq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.daxiang520.top/gtjquxjmcc.html

[Q70] 更新统计信息
来源：http://hz.zhongyouzk.top/gtovhextyq.html

ANALYZE TABLE users;
来源：http://hz.hysaishi.cn/gtzdesbmgy.html

[Q71] 查看建表语句
来源：http://hz.tanke756.top/gtxvdepruq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.bjfxy.top/gtfdfwzpih.html

[Q72] 查看索引
来源：http://hz.ydzc1.top/gtkiasgbcr.html

SHOW INDEX FROM users;
来源：http://hz.hongshengwenyu.top/gtodgmtoic.html

[Q73] 查看表状态
来源：http://hz.daria6918.cn/gtautenclb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ybcxt.top/gtuweahfpz.html

[Q74] 强制使用索引
来源：http://hz.jinqigufen.top/gtgjehysek.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shuidangran.top/gtzmplkaiq.html

[Q75] 日期格式化
来源：http://hz.gotoacloud.top/gtkjjgfpfw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhixingplan.top/gtlxpkvkap.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.birdmap.top/gtxrgxpnbb.html

[Q76] 按天统计
来源：http://hz.dashuyun.cn/gttmvxnuwo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gzhubu.top/gtncqjnljw.html

[Q77] 时间加减
来源：http://hz.cqqwz.cn/gtpwmnrdnf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinqigufen.top/gtsfriarrp.html

[Q78] 当前时间
来源：http://hz.havefunace.top/gtpnlodxen.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.mhx1999.top/gtdkkqsxat.html

[Q79] 字符串拼接
来源：http://hz.zycfv.cn/gtgqpifzqz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj20258.top/gtjzlijqon.html

[Q80] 字符串截取
来源：http://hz.kuanghao11.cn/gtndrmhwsf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tian-w.cn/gtaogofyei.html

[Q81] 字符串替换
来源：http://hz.daria6918.cn/gtmnqvguwr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenjidiqi.icu/gtonyybiht.html

[Q82] 字符长度与字节长度
来源：http://hz.ivvv.top/gtkejuusnx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtwxmayvnb.html

[Q83] 大小写转换
来源：http://hz.feifeiyinyue.top/gtatfckjuk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258888.top/gtvwdskqtd.html

[Q84] 去除首尾空格
来源：http://hz.yuxming.cn/gtjwpuhabb.html

SELECT TRIM(name) FROM users;
来源：http://hz.fengsongda.top/gtohdantvs.html

[Q85] 数值取整
来源：http://hz.52xcode.cn/gtttqgpaak.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gaohongyu789.top/gtzqxqhzbq.html

[Q86] 读取 JSON 字段
来源：http://hz.cashguo.top/gtyilhspzq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinghuilouyu.cn/gtxeocfhrz.html

[Q87] JSON 字段做条件
来源：http://hz.shuidangran.top/gtkjxtjdkm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jlsjyb.cn/gtwatfsvmg.html

[Q88] 行转列（条件聚合）
来源：http://hz.c1oappe.top/gttfrustgi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj20258888.top/gtiueghbba.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.redwolf501.top/gthtrhuskj.html

[Q89] 判断表是否存在
来源：http://hz.52xcode.cn/gtlhexnhjv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangkeji.top/gtpnonthvg.html

[Q90] 生成序号列
来源：http://hz.birdmap.top/gtuuyihlya.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tanke756.top/gtnasuvype.html

================================================================================
来源：http://hz.hywenlv.cn/gtshqgrytr.html

R. Bash 专题
来源：http://hz.hnqzz.top/gtfrriqtpd.html

================================================================================
来源：http://hz.jqgufenzy.top/gtjthpuvux.html

[R01] shebang 与严格模式
来源：http://hz.jyoumei.cn/gthlspzlik.html

#!/usr/bin/env bash
来源：http://hz.guannengcc.top/gtsfuqgnif.html

set -euo pipefail
来源：http://hz.gogol.net.cn/gtkemgiizz.html

[R02] 变量赋值与使用
来源：http://hz.ybcxt.top/gtmedsxdht.html

name="Tom"; echo "$name"
来源：http://hz.xziqi.cn/gtrowlsvjc.html

[R03] 只读变量
来源：http://hz.cqqwz.cn/gtfswmnyvj.html

readonly PI=3.14
来源：http://hz.ppjwa.cn/gtenhaulrg.html

[R04] 位置参数
来源：http://hz.daria6918.cn/gtfavniyjr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.andypj.xyz/gtkasyvugo.html

[R05] 参数默认值
来源：http://hz.nanxinkj.top/gtrtgeoofg.html

name="${1:-default}"
来源：http://hz.yongpay.top/gtirulkwdn.html

[R06] 判断命令是否存在
来源：http://hz.ywan-chungtsiang.top/gthrbsdhnm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.havefunace.top/gteqsryjmn.html

[R07] if 判断文件
来源：http://hz.jqgufenzy.top/gtxuszijcf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.redwolf501.top/gtneitkxyx.html

[R08] 数值比较
来源：http://hz.hfpthk.cn/gtgxhhirjo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cqqwz.cn/gtzmwupjnf.html

[R09] 字符串比较
来源：http://hz.xingfuxueyuan.xyz/gthliqviux.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gaohongyu789.top/gtvcxtafmt.html

[R10] 正则匹配
来源：http://hz.gotoacloud.top/gtfubflubt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hongshengwenyu.top/gtpnbqmapg.html

[R11] case 多分支
来源：http://hz.zhijiandao.cn/gtcffpuujg.html

case "$1" in
来源：http://hz.jiagoushi.top/gteiaaocve.html

start) echo "启动" ;;
来源：http://hz.shzxlz.cn/gtkkbvyyub.html

stop)  echo "停止" ;;
来源：http://hz.cucudq.cn/gtevghcgvr.html

*)     echo "未知命令" ;;
来源：http://hz.jinqigufen.top/gtznlxacus.html

esac
来源：http://hz.xylfe.cn/gtuoufkldv.html

[R12] for 遍历文件
来源：http://hz.chenzaomai.com/gtrdcyezkv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gzhubu.top/gtvxpmzbxq.html

[R13] for 计数循环
来源：http://hz.smart0.xyz/gtkaosdqdv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sweek.top/gtgguyqjrg.html

[R14] C 风格 for
来源：http://hz.gotoacloud.top/gtbqhvumdw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zycfv.cn/gtexqsoxjz.html

[R15] while 逐行读文件
来源：http://hz.shangyingyoupin.top/gtsnpzvvxb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258.top/gtkmexbnob.html

[R16] until 等待条件
来源：http://hz.ivvv.top/gtjnktmqfa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jianghu66.top/gtqirpcivv.html

[R17] 数组定义与取值
来源：http://hz.chenzaomai.com/gthwdwyfij.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenjidiqi.icu/gtfykhmrhj.html

[R18] 遍历数组
来源：http://hz.hfpthk.cn/gtbrheonoe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hnqzz.top/gtvqznhdug.html

[R19] 数组长度
来源：http://hz.chenjidiqi.icu/gtvpmqeqoc.html

echo "${#arr[@]}"
来源：http://hz.hongshengwenyu.top/gttnsgoctp.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtfssdoqme.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hammf.cn/gtxfujvpub.html

[R21] 字符串长度
来源：http://hz.jinqigfzy.top/gtruxfjrht.html

echo "${#s}"
来源：http://hz.gzhubu.top/gtyjnpmusn.html

[R22] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtwdsrpqfg.html

echo "${s:0:5}"
来源：http://hz.yueranfly.top/gtdoeuonub.html

[R23] 字符串替换
来源：http://hz.meibo888.top/gtoeqztiha.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.iojbl.cn/gtustpzwob.html

[R24] 大小写转换
来源：http://hz.snrcjt.cn/gtnguybwde.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.316326.xyz/gtkznpvuex.html

[R25] 去后缀 / 去前缀
来源：http://hz.sweek.top/gttafyhphq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sysykeji.top/gtksgwxhkx.html

[R26] 命令替换
来源：http://hz.wangdashe.top/gtabebutkt.html

now=$(date +%F); echo "$now"
来源：http://hz.wangdashe.top/gthouhhjwc.html

[R27] 算术展开
来源：http://hz.shzxlz.cn/gtincgzfir.html

echo $((1 + 2 * 3))
来源：http://hz.jyoumei.cn/gtjzafeyww.html

[R28] 浮点运算
来源：http://hz.redwolf501.top/gtnhapzfyq.html

echo "scale=2; 10/3" | bc
来源：http://hz.andypj.xyz/gtsyigrfmu.html

[R29] 定义函数
来源：http://hz.vqdsnc.cn/gtzhcqqlbu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cheryme.top/gtbmrpxazz.html

[R30] 函数返回状态码
来源：http://hz.yvedp.cn/gtqdqzyrjg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yangfankeji.com/gtwnsnrwgx.html

[R31] 局部变量
来源：http://hz.cucudq.cn/gteczvvcay.html

f() { local x=1; echo "$x"; }
来源：http://hz.ivvv.top/gtlsxdwrey.html

[R32] 参数个数校验
来源：http://hz.gaohongyu789.top/gtatdnojdu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhengqikj.top/gtmydcwlmc.html

[R33] 捕获错误并提示行号
来源：http://hz.9152youxi.cn/gtsqksqscu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj20258888.top/gtzdljlflc.html

[R34] 退出时清理
来源：http://hz.zhaomingkeji.xyz/gtjxfgohnh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.52xcode.cn/gtfaktgotg.html

[R35] 后台执行并等待
来源：http://hz.nwbrower.top/gtvxobhbhx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnqzz.top/gtjhzzloof.html

[R36] 并发执行多个任务
来源：http://hz.xuanzx.com/gtgqfbrxtu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydjk.org.cn/gthbcixmlc.html

[R37] 把输出赋给变量
来源：http://hz.jianghu66.top/gtcdbszjru.html

files=$(ls -1)
来源：http://hz.yj20258888.top/gtnjryekbr.html

[R38] 管道串联
来源：http://hz.nanxinkj.top/gtqlyfdmom.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daria6918.cn/gtfonrltye.html

[R39] 重定向标准输出与错误
来源：http://hz.jinghuilouyu.cn/gtdacncayq.html

cmd > out.log 2>&1
来源：http://hz.shangyingyoupin.top/gtnwxukzlw.html

[R40] 追加写日志
来源：http://hz.sweek.top/gtqoywlegh.html

echo "log" >> out.log
来源：http://hz.sufxvd.cn/gtmnsfdknc.html

[R41] 丢弃输出
来源：http://hz.yj20258888.top/gtgtxtpkal.html

cmd >/dev/null 2>&1
来源：http://hz.wangshuangyany.cn/gtkhvgojbk.html

[R42] 输入重定向
来源：http://hz.andypj.xyz/gtbmqtygno.html

wc -l < a.txt
来源：http://hz.yj20258.top/gtnmunfsfi.html

[R43] 按名字查找文件
来源：http://hz.zhiwuduotai.top/gtjavtgrcw.html

find . -name "*.log" -type f
来源：http://hz.ywan-chungtsiang.top/gtjecacoeo.html

[R44] 按修改时间查找
来源：http://hz.chenzaomai.com/gtnfkcrqjc.html

find . -mtime -7 -type f
来源：http://hz.hywenlv.cn/gtowcpqmrb.html

[R45] 批量删除
来源：http://hz.zhaomingkeji.xyz/gtdwhyybyc.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangkeji.top/gtmrlapwbb.html

[R46] 递归替换文件内容
来源：http://hz.daria6918.cn/gtcneuxika.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xinyue.icu/gtkszkoctf.html

[R47] sed 单行替换
来源：http://hz.ywan-chungtsiang.top/gtxueripkb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.andypj.xyz/gtevqndcif.html

[R48] awk 取指定列
来源：http://hz.ppjwa.cn/gtkgvvamle.html

awk '{print $1, $3}' a.txt
来源：http://hz.cheryme.top/gtkcadundm.html

[R49] awk 带条件
来源：http://hz.hysaishi.cn/gtskdrjyuu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258888.top/gtqrsoepvq.html

[R50] awk 求和
来源：http://hz.zhixingplan.top/gtoevemisd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sxryk.cn/gtjlhdphfx.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gtcczyyebr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sxryk.cn/gtechgalee.html

[R52] 统计行数
来源：http://hz.yanxiufei.cn/gtsbgmtixe.html

wc -l a.txt
来源：http://hz.0kj1m.cn/gtnwguzlbh.html

[R53] 查看文件头与实时尾
来源：http://hz.nanxinkj.top/gtgpemsexe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.meibo888.top/gtmvkouqiu.html

[R54] 比较两个文件
来源：http://hz.chenlongwang.top/gtyzlylcaq.html

diff a.txt b.txt
来源：http://hz.meibo888.top/gtivinwmut.html

[R55] 压缩与解压
来源：http://hz.cheryme.top/gtkstuuybd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sweek.top/gtbjaxishc.html

[R56] 远程拷贝
来源：http://hz.yj202588.top/gtagrlubjl.html

scp file user@host:/path/
来源：http://hz.yongpay.top/gtmkswazoy.html

[R57] 远程执行命令
来源：http://hz.smart0.xyz/gtcthhxywh.html

ssh user@host 'uptime'
来源：http://hz.gogol.net.cn/gtlxyukfob.html

[R58] 下载文件
来源：http://hz.jyoumei.cn/gtsbqnapek.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.bjfxy.top/gtlagfzllh.html

[R59] 发 POST JSON
来源：http://hz.chenlongwang.top/gtfylqqzji.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.daria6918.cn/gtfuavgnsm.html

[R60] 只看 HTTP 状态码
来源：http://hz.yongpay.top/gtoxfsgliy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.vqdsnc.cn/gtroazjonf.html

[R61] 磁盘占用
来源：http://hz.aizwys.cn/gtebckjuao.html

df -h;  du -sh *
来源：http://hz.jiagoushi.top/gtwzjhayar.html

[R62] 找最占空间的文件
来源：http://hz.daria6918.cn/gtwmazwwfa.html

du -ah . | sort -rh | head -10
来源：http://hz.wangshuangyany.cn/gttqyvbxwg.html

[R63] 内存与进程
来源：http://hz.zhijiandao.cn/gtnycmfszr.html

free -h;  ps aux | grep nginx
来源：http://hz.yonumen.top/gtpjuyvbhb.html

[R64] 结束进程
来源：http://hz.daxiang520.top/gtcvplnngo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.bjfxy.top/gtlfutgpep.html

[R65] 查看端口占用
来源：http://hz.yuanzhike.top/gtofmicinw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.redwolf501.top/gtlylphzrf.html

[R66] 定时任务
来源：http://hz.c1oappe.top/gtzrafzlxq.html

crontab -e;  crontab -l
来源：http://hz.sweek.top/gtzuwzrjpz.html

[R67] 生成随机十六进制串
来源：http://hz.havefunace.top/gtlnpindle.html

openssl rand -hex 16
来源：http://hz.sysykeji.top/gteplfzjak.html

[R68] 计算文件校验值
来源：http://hz.yongpay.top/gtmzxssjlg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.0kj1m.cn/gttfofngnf.html

[R69] 生成随机密码
来源：http://hz.hywenlv.cn/gtaiaerndj.html

head -c 16 /dev/urandom | base64
来源：http://hz.hammf.cn/gtqbvwnyin.html

[R70] 时间戳与互转
来源：http://hz.hfpthk.cn/gtzfffymua.html

date +%s;  date -d @1700000000
来源：http://hz.xuanzx.com/gtlfjqaznw.html

[R71] 日期格式化
来源：http://hz.aizwys.cn/gtmaktkycx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ppjwa.cn/gtzhtdhqqq.html

[R72] 等待端口就绪
来源：http://hz.aizwys.cn/gtpxxouill.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.birdmap.top/gtqgxhujah.html

[R73] 分割大日志
来源：http://hz.xylfe.cn/gtptvieqsx.html

split -l 1000 big.log part_
来源：http://hz.chenlongwang.top/gtfwfugyli.html

[R74] 批量重命名
来源：http://hz.vqdsnc.cn/gtshkkpwkh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yuanzhike.top/gtlhcfrhzc.html

[R75] 导出环境变量
来源：http://hz.yueranfly.top/gtexmfgehi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tianlin.xyz/gtvlvukfbg.html

[R76] 使用临时文件
来源：http://hz.fzhhl.top/gtnqaquqgh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ivvv.top/gtacppyzlz.html

[R77] 读取用户输入
来源：http://hz.ehwqpu.com/gtiyzvcsad.html

read -rp "请输入: " ans
来源：http://hz.jqgfzy.top/gtvlkysuxm.html

[R78] 交互式菜单
来源：http://hz.yangfankeji.com/gtdtojzxoq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yuanzhike.top/gtgxamjnrt.html

[R79] 解析命令行选项
来源：http://hz.birdmap.top/gtqwsxzpsu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sysykeji.top/gtsgqgzuue.html

[R80] 查看脚本执行耗时
来源：http://hz.redwolf501.top/gtgznhvklb.html

time ./run.sh
来源：http://hz.hongshengwenyu.top/gtqnnsjpur.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtiulkcmyn.html

S. C / C++ 专题
来源：http://hz.daria6918.cn/gtiopvjspx.html

================================================================================
来源：http://hz.jinqigufen.top/gtiqlrwzcj.html

[S01] C：Hello World
来源：http://hz.zhaomingkeji.xyz/gtkekvayiq.html

#include <stdio.h>
来源：http://hz.zhiwuduotai.top/gtcooryhnt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.pengpengdd.cyou/gtdxaqqkri.html

[S02] C：变量与格式化输出
来源：http://hz.yangfankeji.com/gtpzvjtyvz.html

int a = 10; printf("%d\n", a);
来源：http://hz.jianghu66.top/gtbclfkhct.html

[S03] C：读入整数
来源：http://hz.tanke756.top/gtwnsoobrs.html

int x; scanf("%d", &x);
来源：http://hz.tianlin.xyz/gtgtzgmfwo.html

[S04] C：字符串复制
来源：http://hz.yongpay.top/gtpbycaevh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.smart0.xyz/gtskyglkde.html

[S05] C：字符串长度
来源：http://hz.bjfxy.top/gtuxmvkogc.html

strlen(s)
来源：http://hz.nwbrower.top/gtvwazgddq.html

[S06] C：字符串比较
来源：http://hz.zhaomingkeji.xyz/gthbhnnvhh.html

strcmp(a, b) == 0
来源：http://hz.c1oappe.top/gtuvrrhqpu.html

[S07] C：数组遍历求和
来源：http://hz.iojbl.cn/gtopnfhoap.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhaomingkeji.xyz/gtsnkblajz.html

[S08] C：动态内存分配与释放
来源：http://hz.meibo888.top/gtstquxiwm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tianlin.xyz/gtancxxgdg.html

[S09] C：结构体定义与初始化
来源：http://hz.yj202588.top/gtypojtsuh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinqigfzy.top/gttyprwogn.html

[S10] C：指针与解引用
来源：http://hz.gaohongyu789.top/gtsgfpzwbw.html

int *p = &a;  *p = 5;
来源：http://hz.tianlin.xyz/gtfxyciror.html

[S11] C：逐行读文件
来源：http://hz.meibo888.top/gtnsoahxjh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhixingplan.top/gtdhbxnqjq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nwbrower.top/gtepraacny.html

fclose(f);
来源：http://hz.fzhhl.top/gtvpbcyroy.html

[S12] C：写文件
来源：http://hz.kuanghao11.cn/gtfgdozxtz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gotoacloud.top/gtlsevpzse.html

[S13] C：宏定义
来源：http://hz.yueranfly.top/gtapyvavvy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.mhx1999.top/gtoewwguds.html

[S14] C：枚举
来源：http://hz.guannengcc.top/gtbcihxdno.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hongshengwenyu.top/gthtrmswkb.html

[S15] C：类型转换
来源：http://hz.jinyuanbaomall.cn/gtzsozzimb.html

(double) a / b
来源：http://hz.ehwqpu.com/gtzpxejmzi.html

[S16] C：位操作置位
来源：http://hz.ydzc1.top/gtufoccueg.html

x |= (1 << 3);
来源：http://hz.jqgufenzy.top/gtenfxlqvu.html

[S17] C：安全拼接字符串
来源：http://hz.feifeiyinyue.top/gtrmxcwnjj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangdashe.top/gtaqkgdxiz.html

[S18] C：命令行参数
来源：http://hz.pycfn.com/gtcbexxylx.html


<!-- 参考信息 -->