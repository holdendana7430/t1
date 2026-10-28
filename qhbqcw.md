代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ybcxt.top/gtckzihoow.html

[Q50] 批量更新
来源：http://hz.jinqigufen.top/gtxdvshpqy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.tian-w.cn/gtaptkgcue.html

[Q51] 用子查询更新
来源：http://hz.yuanzhike.top/gtsdwcyatr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yvedp.cn/gtxthnragg.html

[Q52] 删除指定行
来源：http://hz.shzxlz.cn/gtdywkigkt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nwbrower.top/gtqcudcaba.html

[Q53] 按条件删除
来源：http://hz.zhongyouzk.top/gtmvbsnsdq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinqigfzy.top/gtsexfvkvs.html

[Q54] 清空表
来源：http://hz.andypj.xyz/gthkfcmihw.html

TRUNCATE TABLE logs;
来源：http://hz.sysykeji.top/gtketyhoqf.html

[Q55] 排名（并列占位）
来源：http://hz.ywan-chungtsiang.top/gtrkdkxzmt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xziqi.cn/gtbdussdtq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pengpengdd.cyou/gtynnbusjh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yvedp.cn/gtafsmaodp.html

[Q57] 行号
来源：http://hz.guannengcc.top/gttiiioeoy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgfzy.top/gtkmoxbawd.html

[Q58] 累计求和
来源：http://hz.xuetiantiany.cn/gtiiqvtvzd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhiwuduotai.top/gtvwzfzhkq.html

[Q59] 分组内累计
来源：http://hz.yueranfly.top/gtnhrirtze.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gthopgmwks.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhijiandao.cn/gtfnzjcvdc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinghuilouyu.cn/gtmpjbctjg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.kuanghao11.cn/gtdiaekhdc.html

[Q61] 移动平均
来源：http://hz.shzxlz.cn/gtymulmxui.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangdashe.top/gtpxhdukff.html

[Q62] 分组占比
来源：http://hz.cdnleiting.top/gtljdrlatf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtmkwcnikc.html

[Q63] 开启事务
来源：http://hz.cqqwz.cn/gtfnmothar.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.havefunace.top/gtpgimqgsf.html

[Q64] 提交事务
来源：http://hz.fzhhl.top/gtsvwgfffq.html

COMMIT;
来源：http://hz.xziqi.cn/gtlxgjnmoj.html

[Q65] 回滚事务
来源：http://hz.gzhubu.top/gtrlccanym.html

ROLLBACK;
来源：http://hz.zhiwuduotai.top/gtkytsjbng.html

[Q66] 行锁查询
来源：http://hz.meibo888.top/gthyoegbjp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ybcxt.top/gtbcmiswwo.html

[Q67] 设置隔离级别
来源：http://hz.shanyushiyangkeji.top/gttzmhrrnt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jianghu66.top/gtenrrrirt.html

[Q68] 保存点
来源：http://hz.zhaomingkeji.xyz/gtypmxlewt.html

SAVEPOINT sp1;
来源：http://hz.wangdashe.top/gtgesvazoz.html

ROLLBACK TO sp1;
来源：http://hz.ppjwa.cn/gtcakbuigo.html

[Q69] 查看执行计划
来源：http://hz.yuxming.cn/gtcdpyztoo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jianghu66.top/gtzlqvuobr.html

[Q70] 更新统计信息
来源：http://hz.jiagoushi.top/gtsbqdbrsh.html

ANALYZE TABLE users;
来源：http://hz.yangfankeji.com/gtdzwwkher.html

[Q71] 查看建表语句
来源：http://hz.shzxlz.cn/gtmrxgbfer.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.svipenyu.cn/gtkabvqxzo.html

[Q72] 查看索引
来源：http://hz.xziqi.cn/gtvtbkzbhz.html

SHOW INDEX FROM users;
来源：http://hz.dashuyun.cn/gtzxdowtca.html

[Q73] 查看表状态
来源：http://hz.svipenyu.cn/gthcnnsbdi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hammf.cn/gtwqgccgxf.html

[Q74] 强制使用索引
来源：http://hz.shzxlz.cn/gtybfbfsno.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigfzy.top/gtgrbxukmv.html

[Q75] 日期格式化
来源：http://hz.ehwqpu.com/gtpaxzjxau.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.feifeiyinyue.top/gtpsadyehk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangdashe.top/gtkikeakqv.html

[Q76] 按天统计
来源：http://hz.cdnleiting.top/gtqrykedmy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.c1oappe.top/gthdklrfxi.html

[Q77] 时间加减
来源：http://hz.aibaodan.cn/gtpvdvwrza.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zycfv.cn/gtzrjrxbfp.html

[Q78] 当前时间
来源：http://hz.316326.xyz/gtwnadfhja.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xuetiantiany.cn/gtflzuizdp.html

[Q79] 字符串拼接
来源：http://hz.yvedp.cn/gtxpxyypfr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhiwuduotai.top/gtybblhetk.html

[Q80] 字符串截取
来源：http://hz.fzhhl.top/gtxquyvitk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.guannengcc.top/gtnnfgutmo.html

[Q81] 字符串替换
来源：http://hz.ehwqpu.com/gtvriwedxj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhijiandao.cn/gtjorbmves.html

[Q82] 字符长度与字节长度
来源：http://hz.hywenlv.cn/gtznopzpfq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtmjxcclht.html

[Q83] 大小写转换
来源：http://hz.hfpthk.cn/gtbzifyhtg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sysykeji.top/gtdfualleb.html

[Q84] 去除首尾空格
来源：http://hz.sxryk.cn/gtbmunvlli.html

SELECT TRIM(name) FROM users;
来源：http://hz.cdnleiting.top/gtvjwdtdpp.html

[Q85] 数值取整
来源：http://hz.sweek.top/gtdcxzhdux.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ydjk.org.cn/gtfhzmunuo.html

[Q86] 读取 JSON 字段
来源：http://hz.andypj.xyz/gtomldylzi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.pycfn.com/gtapuououg.html

[Q87] JSON 字段做条件
来源：http://hz.zhongyouzk.top/gtxmecozmi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gogol.net.cn/gtrohohpav.html

[Q88] 行转列（条件聚合）
来源：http://hz.cheryme.top/gtywwzvbjo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shangyingyoupin.top/gtknxetlck.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinyuanbaomall.cn/gthdygtaab.html

[Q89] 判断表是否存在
来源：http://hz.52xcode.cn/gtjfnxsodw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ehwqpu.com/gtvdampjxu.html

[Q90] 生成序号列
来源：http://hz.zhengqikj.top/gtdklrphwa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cashguo.top/gtzftyjsvq.html

================================================================================
来源：http://hz.jyoumei.cn/gtauifoqqv.html

R. Bash 专题
来源：http://hz.zhiwuduotai.top/gtqmeqfovr.html

================================================================================
来源：http://hz.snrcjt.cn/gtvtitjnhl.html

[R01] shebang 与严格模式
来源：http://hz.kuanghao11.cn/gtqscdsnqb.html

#!/usr/bin/env bash
来源：http://hz.yvedp.cn/gtlyznargo.html

set -euo pipefail
来源：http://hz.tanke756.top/gtmimchijr.html

[R02] 变量赋值与使用
来源：http://hz.jqgufenzy.top/gtserlxnek.html

name="Tom"; echo "$name"
来源：http://hz.zhengqikj.top/gtvwyuobuu.html

[R03] 只读变量
来源：http://hz.hnxiangtu.top/gtqoxdxvhy.html

readonly PI=3.14
来源：http://hz.wangshuangyany.cn/gtbybjnttu.html

[R04] 位置参数
来源：http://hz.feifeiyinyue.top/gtmdrqewll.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangshuangyany.cn/gtamxybjlr.html

[R05] 参数默认值
来源：http://hz.yangfankeji.com/gtmtipesfs.html

name="${1:-default}"
来源：http://hz.yj20258.top/gtdpqrqlmy.html

[R06] 判断命令是否存在
来源：http://hz.yongpay.top/gtrlgjizwg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.mhx1999.top/gtmthrfioq.html

[R07] if 判断文件
来源：http://hz.cashguo.top/gtgiqioezx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhijiandao.cn/gtkvjlyjlg.html

[R08] 数值比较
来源：http://hz.yueranfly.top/gtfqrsxffd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.aibaodan.cn/gtitqxjrxv.html

[R09] 字符串比较
来源：http://hz.chenjidiqi.icu/gtzqljwump.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tianlin.xyz/gtrixgozvu.html

[R10] 正则匹配
来源：http://hz.ybcxt.top/gtkdxvyuii.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ydjk.org.cn/gtsvydqtgp.html

[R11] case 多分支
来源：http://hz.pengpengdd.cyou/gtdlitmisb.html

case "$1" in
来源：http://hz.yj20258888.top/gthcuxrnnh.html

start) echo "启动" ;;
来源：http://hz.sweek.top/gtgczmrisw.html

stop)  echo "停止" ;;
来源：http://hz.yuanzhike.top/gtkenqimgb.html

*)     echo "未知命令" ;;
来源：http://hz.sysykeji.top/gtqmxtried.html

esac
来源：http://hz.jinghuilouyu.cn/gtbrylkkfk.html

[R12] for 遍历文件
来源：http://hz.ivvv.top/gtrscyslvc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.daxiang520.top/gtxohmiovn.html

[R13] for 计数循环
来源：http://hz.daxiang520.top/gtyzxkhoid.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shuidangran.top/gtmkcwqhqr.html

[R14] C 风格 for
来源：http://hz.gzhubu.top/gtfivzuhcw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhijiandao.cn/gtxrpbjhol.html

[R15] while 逐行读文件
来源：http://hz.yueranfly.top/gttstlaiko.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuxming.cn/gtbwiyirki.html

[R16] until 等待条件
来源：http://hz.zhijiandao.cn/gtytugansj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtfcutannx.html

[R17] 数组定义与取值
来源：http://hz.yangfankeji.com/gtbwbpotmw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.guannengcc.top/gtxporbaid.html

[R18] 遍历数组
来源：http://hz.yanxiufei.cn/gtnvlhnwlk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.havefunace.top/gtpgyapwln.html

[R19] 数组长度
来源：http://hz.iojbl.cn/gtoebgeuqj.html

echo "${#arr[@]}"
来源：http://hz.yuanzhike.top/gtapmppjps.html

[R20] 关联数组（字典）
来源：http://hz.chenjidiqi.icu/gtaofgtodv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tanke756.top/gtvcdhzpsx.html

[R21] 字符串长度
来源：http://hz.jyoumei.cn/gtekxztejr.html

echo "${#s}"
来源：http://hz.fengsongda.top/gtnugpiosn.html

[R22] 截取子串
来源：http://hz.cdnleiting.top/gtjntyxqml.html

echo "${s:0:5}"
来源：http://hz.jqgfzy.top/gtiyrnecsr.html

[R23] 字符串替换
来源：http://hz.jqgfzy.top/gtmglwoejk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yongpay.top/gtkqqmdgrc.html

[R24] 大小写转换
来源：http://hz.aizwys.cn/gtdpzumfov.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hysaishi.cn/gtbstqevjj.html

[R25] 去后缀 / 去前缀
来源：http://hz.hammf.cn/gtrbmgqrjh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.0kj1m.cn/gtwjplsycb.html

[R26] 命令替换
来源：http://hz.dashuyun.cn/gtjvamfwcc.html

now=$(date +%F); echo "$now"
来源：http://hz.yvedp.cn/gtapxdxevr.html

[R27] 算术展开
来源：http://hz.gzhubu.top/gtyudvtfyw.html

echo $((1 + 2 * 3))
来源：http://hz.chenjidiqi.icu/gtpzhkatri.html

[R28] 浮点运算
来源：http://hz.xylfe.cn/gtktcxumus.html

echo "scale=2; 10/3" | bc
来源：http://hz.jqgfzy.top/gtfguuewnm.html

[R29] 定义函数
来源：http://hz.ppjwa.cn/gtpihzoghx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhengqikj.top/gtkjeikyqm.html

[R30] 函数返回状态码
来源：http://hz.nanxinkj.top/gtqpzarofx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.dashuyun.cn/gtpykstdlc.html

[R31] 局部变量
来源：http://hz.pycfn.com/gtywjqfcxh.html

f() { local x=1; echo "$x"; }
来源：http://hz.ehwqpu.com/gtehpakzrk.html

[R32] 参数个数校验
来源：http://hz.shangyingyoupin.top/gtrahlhrvv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sysykeji.top/gtxjvqrsym.html

[R33] 捕获错误并提示行号
来源：http://hz.havefunace.top/gtpvdsoboj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jyoumei.cn/gtepqbcypq.html

[R34] 退出时清理
来源：http://hz.yj20258.top/gtlwdmrvhg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jianghu66.top/gtrvdvkqzp.html

[R35] 后台执行并等待
来源：http://hz.smart0.xyz/gtiofltrki.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnxiangtu.top/gtjvguzezq.html

[R36] 并发执行多个任务
来源：http://hz.zhengqikj.top/gthyuylyxt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhengqikj.top/gtrlaeiihp.html

[R37] 把输出赋给变量
来源：http://hz.sufxvd.cn/gtzpecierm.html

files=$(ls -1)
来源：http://hz.nanxuanxn.top/gttdibirnx.html

[R38] 管道串联
来源：http://hz.nanxinkj.top/gtwcjpcffn.html

cat a.txt | grep -i error | wc -l
来源：http://hz.meibo888.top/gtuygouqtd.html

[R39] 重定向标准输出与错误
来源：http://hz.meibo888.top/gtvxuxdewj.html

cmd > out.log 2>&1
来源：http://hz.jinghuilouyu.cn/gtjfbffjag.html

[R40] 追加写日志
来源：http://hz.52xcode.cn/gthrlkkxgn.html

echo "log" >> out.log
来源：http://hz.vqdsnc.cn/gtcwawcklv.html

[R41] 丢弃输出
来源：http://hz.52xcode.cn/gtytsbprab.html

cmd >/dev/null 2>&1
来源：http://hz.zhoulong.xyz/gtrmrrqsuf.html

[R42] 输入重定向
来源：http://hz.ybcxt.top/gtygxqckde.html

wc -l < a.txt
来源：http://hz.dashuyun.cn/gtyvqfndrf.html

[R43] 按名字查找文件
来源：http://hz.chenlongwang.top/gtwxvruagu.html

find . -name "*.log" -type f
来源：http://hz.daxiang520.top/gtokiepcye.html

[R44] 按修改时间查找
来源：http://hz.bjfxy.top/gtbmjaombt.html

find . -mtime -7 -type f
来源：http://hz.316326.xyz/gtciotewhd.html

[R45] 批量删除
来源：http://hz.hnxiangtu.top/gtawdkotxu.html

find . -name "*.tmp" -delete
来源：http://hz.aizwys.cn/gtfhqazhtd.html

[R46] 递归替换文件内容
来源：http://hz.zhengqikj.top/gtfjbzaekc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhaomingkeji.xyz/gtlonpydit.html

[R47] sed 单行替换
来源：http://hz.smart0.xyz/gtctumluev.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yonumen.top/gtrxadmaey.html

[R48] awk 取指定列
来源：http://hz.cucudq.cn/gthqyvpyis.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuetiantiany.cn/gtmmjcgpla.html

[R49] awk 带条件
来源：http://hz.ywan-chungtsiang.top/gtvetvpbjo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.meibo888.top/gtylnteppo.html

[R50] awk 求和
来源：http://hz.yangfankeji.com/gtatvagloa.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hysaishi.cn/gtfedajkyp.html

[R51] 排序去重取前几
来源：http://hz.xylfe.cn/gtvbutnxdk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gaohongyu789.top/gtyareqzqt.html

[R52] 统计行数
来源：http://hz.ydjk.org.cn/gtdhbaekrb.html

wc -l a.txt
来源：http://hz.c1oappe.top/gtoykydouk.html

[R53] 查看文件头与实时尾
来源：http://hz.zhengqikj.top/gtblvzhver.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xylfe.cn/gtipohimxn.html

[R54] 比较两个文件
来源：http://hz.jiagoushi.top/gtpndnyuqt.html

diff a.txt b.txt
来源：http://hz.wangdashe.top/gtbtslgqsg.html

[R55] 压缩与解压
来源：http://hz.xuetiantiany.cn/gtwetamjet.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yongpay.top/gtyooqymup.html

[R56] 远程拷贝
来源：http://hz.jlsjyb.cn/gtwqqweczl.html

scp file user@host:/path/
来源：http://hz.fzhhl.top/gthsafqmqz.html

[R57] 远程执行命令
来源：http://hz.ehwqpu.com/gterfieowv.html

ssh user@host 'uptime'
来源：http://hz.shanyushiyangtech.top/gtmswqlnju.html

[R58] 下载文件
来源：http://hz.ivvv.top/gtyrwzgmzq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.kuanghao11.cn/gtuxuspqfi.html

[R59] 发 POST JSON
来源：http://hz.ywan-chungtsiang.top/gtcciexfqm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.redwolf501.top/gtglwumrqa.html

[R60] 只看 HTTP 状态码
来源：http://hz.cheryme.top/gttfqhryzu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cashguo.top/gtnhgwkqea.html

[R61] 磁盘占用
来源：http://hz.yongpay.top/gtteuzfrzb.html

df -h;  du -sh *
来源：http://hz.cqqwz.cn/gtdaspmtov.html

[R62] 找最占空间的文件
来源：http://hz.jinqigfzy.top/gtwkijpevh.html

du -ah . | sort -rh | head -10
来源：http://hz.ydjk.org.cn/gteikgzlaa.html

[R63] 内存与进程
来源：http://hz.jqgfzy.top/gtpgdhatdx.html

free -h;  ps aux | grep nginx
来源：http://hz.shuidangran.top/gtilrnngbu.html

[R64] 结束进程
来源：http://hz.sufxvd.cn/gtmiriwaxa.html

kill -9 $(pgrep -f app.py)
来源：http://hz.fengsongda.top/gtgvnabppt.html

[R65] 查看端口占用
来源：http://hz.guowangkeji.top/gtdgnbhxma.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jianghu66.top/gtobospifm.html

[R66] 定时任务
来源：http://hz.hnqzz.top/gtxlflcqcq.html

crontab -e;  crontab -l
来源：http://hz.cucudq.cn/gtrnonezzn.html

[R67] 生成随机十六进制串
来源：http://hz.guowangkeji.top/gtdighixbz.html

openssl rand -hex 16
来源：http://hz.yuanzhike.top/gtkdxzefhz.html

[R68] 计算文件校验值
来源：http://hz.chenlongwang.top/gtsichidvh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtsnvzfjao.html

[R69] 生成随机密码
来源：http://hz.chenlongwang.top/gttcadpoxp.html

head -c 16 /dev/urandom | base64
来源：http://hz.dianchejie.cn/gtmsdzdaoh.html

[R70] 时间戳与互转
来源：http://hz.jinqigfzy.top/gtvbbiafzl.html

date +%s;  date -d @1700000000
来源：http://hz.nanxinkj.top/gtdaqzbjoz.html

[R71] 日期格式化
来源：http://hz.wangdashe.top/gtxwschdxo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhiwuduotai.top/gtpzefvqur.html

[R72] 等待端口就绪
来源：http://hz.hysaishi.cn/gtnqcrwzud.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.c1oappe.top/gtdaewzvlg.html

[R73] 分割大日志
来源：http://hz.svipenyu.cn/gtnkraqhnl.html

split -l 1000 big.log part_
来源：http://hz.yangfankeji.com/gtvueyiern.html

[R74] 批量重命名
来源：http://hz.c1oappe.top/gtpznljlxi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.birdmap.top/gtsvutjrkx.html

[R75] 导出环境变量
来源：http://hz.wangdashe.top/gtlsfqgxwg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shuidangran.top/gtvglyisjs.html

[R76] 使用临时文件
来源：http://hz.yuxming.cn/gtidfzawnt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinyuanbaomall.cn/gtxkvtijme.html

[R77] 读取用户输入
来源：http://hz.hongshengwenyu.top/gtgaiepvhu.html

read -rp "请输入: " ans
来源：http://hz.nanxinkj.top/gtnkmmojgl.html

[R78] 交互式菜单
来源：http://hz.zhixingplan.top/gtqujtabbv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhixingplan.top/gtindstuis.html

[R79] 解析命令行选项
来源：http://hz.xuetiantiany.cn/gtssykvcuq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.9152youxi.cn/gtiirsdjku.html

[R80] 查看脚本执行耗时
来源：http://hz.meibo888.top/gtufxssyss.html

time ./run.sh
来源：http://hz.svipenyu.cn/gtwfwmlkmj.html

================================================================================
来源：http://hz.jinqigfzy.top/gtyyxrbpgr.html

S. C / C++ 专题
来源：http://hz.hongshengwenyu.top/gtzzvjccep.html

================================================================================
来源：http://hz.hywenlv.cn/gtegpayfye.html

[S01] C：Hello World
来源：http://hz.tianlin.xyz/gtioxnltvt.html

#include <stdio.h>
来源：http://hz.cashguo.top/gtbaeillsg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.birdmap.top/gtpxtauonc.html

[S02] C：变量与格式化输出
来源：http://hz.cdnleiting.top/gtykpeywwh.html

int a = 10; printf("%d\n", a);
来源：http://hz.kuanghao11.cn/gtcfaoiaee.html

[S03] C：读入整数
来源：http://hz.nanxuanxn.top/gtjlswnycv.html

int x; scanf("%d", &x);
来源：http://hz.52xcode.cn/gtbltotyyq.html

[S04] C：字符串复制
来源：http://hz.yvedp.cn/gtjcbvylcm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jiagoushi.top/gthbdszwsk.html

[S05] C：字符串长度
来源：http://hz.kuanghao11.cn/gtdtssggzc.html

strlen(s)
来源：http://hz.yj20258888.top/gtvmmvjmzz.html

[S06] C：字符串比较
来源：http://hz.sysykeji.top/gtksomlium.html

strcmp(a, b) == 0
来源：http://hz.hfpthk.cn/gtqadokegt.html

[S07] C：数组遍历求和
来源：http://hz.cucudq.cn/gtquzsqrcr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.daxiang520.top/gtkghpbgfj.html

[S08] C：动态内存分配与释放
来源：http://hz.sysykeji.top/gtshtuziww.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.snrcjt.cn/gtbhmgotlq.html

[S09] C：结构体定义与初始化
来源：http://hz.zhengqikj.top/gtcckxjadv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.pengpengdd.cyou/gtuxtveahy.html

[S10] C：指针与解引用
来源：http://hz.yuanzhike.top/gtwrsdgvze.html

int *p = &a;  *p = 5;
来源：http://hz.jyoumei.cn/gticzxalrd.html

[S11] C：逐行读文件
来源：http://hz.yj202588.top/gttntjthox.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jlsjyb.cn/gtoypauntp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinghuilouyu.cn/gttbgjyduj.html

fclose(f);
来源：http://hz.dianchejie.cn/gtszzvgbdd.html

[S12] C：写文件
来源：http://hz.zdqjudy.top/gtfqjccbxt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.guannengcc.top/gtbnqqrhlq.html

[S13] C：宏定义
来源：http://hz.aibaodan.cn/gtgxdrdtiv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuanzhike.top/gtkbasieib.html

[S14] C：枚举
来源：http://hz.jinyuanbaomall.cn/gtnmtzrcst.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hammf.cn/gtcoomjzjv.html

[S15] C：类型转换
来源：http://hz.andypj.xyz/gtldvmfyho.html

(double) a / b
来源：http://hz.xinyue.icu/gtgxbuepxn.html

[S16] C：位操作置位
来源：http://hz.iojbl.cn/gtatgizckj.html

x |= (1 << 3);
来源：http://hz.zhoulong.xyz/gtkhkfxpsg.html

[S17] C：安全拼接字符串
来源：http://hz.hfpthk.cn/gtlkalxygz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shangyingyoupin.top/gtisshamcz.html

[S18] C：命令行参数
来源：http://hz.tanke756.top/gtkdblijve.html

int main(int argc, char **argv)
来源：http://hz.ehwqpu.com/gtqqxgnyar.html

[S19] C：快速排序
来源：http://hz.zdqjudy.top/gtvtsyvokq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.meibo888.top/gtqrqizmwy.html

[S20] C：二分查找
来源：http://hz.ydzc1.top/gtblqzmzfn.html


<!-- 参考信息 -->