代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.316326.xyz/gtpuwjdlir.html

JOIN users u ON u.id = o.user_id
来源：http://hz.redwolf501.top/gtbdqtnqff.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.pycfn.com/gtohdsszzv.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgufenzy.top/gtrdwvmrlu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gogol.net.cn/gtvuhksaod.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gzhubu.top/gtgcvwhszv.html

[Q43] 标量子查询
来源：http://hz.tanke756.top/gtflxmjkob.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shanyushiyangtech.top/gtrppqpvqy.html

[Q44] IN 子查询
来源：http://hz.ywan-chungtsiang.top/gtlsaqqvrm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.iojbl.cn/gtnxvcgkdw.html

[Q45] EXISTS 判断存在
来源：http://hz.nanxinkj.top/gtidakpiai.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgufenzy.top/gtinzjfaxl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.tianlin.xyz/gtzfefwjmo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.316326.xyz/gtiuwetdap.html

[Q47] 与平均值比较
来源：http://hz.hnxiangtu.top/gtribfetov.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yonumen.top/gtgzrmltkv.html

[Q48] CTE 公用表表达式
来源：http://hz.hywenlv.cn/gtagvosrpn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.mhx1999.top/gtmlilewbf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.snrcjt.cn/gterzvlyxj.html

[Q49] 更新单行
来源：http://hz.havefunace.top/gttpgyhqss.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xuetiantiany.cn/gtwinbwtms.html

[Q50] 批量更新
来源：http://hz.yj202588.top/gthsjrsaxe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenlongwang.top/gtwqdcgzhd.html

[Q51] 用子查询更新
来源：http://hz.quarkkingdee.top/gtdpouskgw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.0kj1m.cn/gtrwfwxfkj.html

[Q52] 删除指定行
来源：http://hz.ehwqpu.com/gtlytnbfhc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ybcxt.top/gtgkhiikap.html

[Q53] 按条件删除
来源：http://hz.jiagoushi.top/gtmtocqjze.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tanke756.top/gtuqfxevsi.html

[Q54] 清空表
来源：http://hz.mhx1999.top/gtmlcdzcpy.html

TRUNCATE TABLE logs;
来源：http://hz.jqgfzy.top/gtotievjea.html

[Q55] 排名（并列占位）
来源：http://hz.cucudq.cn/gtbtlthdda.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.chenlongwang.top/gtclhtxptc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhiwuduotai.top/gtjnhkibha.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj20258.top/gtvmmbcbog.html

[Q57] 行号
来源：http://hz.ehwqpu.com/gtvviuszbv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgfzy.top/gtrjbcplnw.html

[Q58] 累计求和
来源：http://hz.zdqjudy.top/gtgbdtkhzx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cucudq.cn/gtjorhnbjj.html

[Q59] 分组内累计
来源：http://hz.yuxming.cn/gthusxojjx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gtivzuzyia.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhixingplan.top/gtyqipapxp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xingfuxueyuan.xyz/gtoqbebtwv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zdqjudy.top/gtlvkgupdg.html

[Q61] 移动平均
来源：http://hz.nanxuanxn.top/gtccsrowxz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sufxvd.cn/gtpljxjmrr.html

[Q62] 分组占比
来源：http://hz.andypj.xyz/gtgahgcoea.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.svipenyu.cn/gtzkmqkxup.html

[Q63] 开启事务
来源：http://hz.hywenlv.cn/gtxrgrszqh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.iojbl.cn/gtasxiffwj.html

[Q64] 提交事务
来源：http://hz.shangyingyoupin.top/gtkteqqtyy.html

COMMIT;
来源：http://hz.hnxiangtu.top/gtyxzbytzd.html

[Q65] 回滚事务
来源：http://hz.nanxinkj.top/gttitlmmfm.html

ROLLBACK;
来源：http://hz.gotoacloud.top/gtcczgdydp.html

[Q66] 行锁查询
来源：http://hz.wangdashe.top/gtldhigsrp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pengpengdd.cyou/gtdqdbgwve.html

[Q67] 设置隔离级别
来源：http://hz.svipenyu.cn/gtwkyxbwbr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jianghu66.top/gthnwyhtxb.html

[Q68] 保存点
来源：http://hz.haohaochexian.top/gtkxaakezn.html

SAVEPOINT sp1;
来源：http://hz.yj20258888.top/gtulmvxdie.html

ROLLBACK TO sp1;
来源：http://hz.pengpengdd.cyou/gtlwkyjyzk.html

[Q69] 查看执行计划
来源：http://hz.iojbl.cn/gtteinapdw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jlsjyb.cn/gtuzwkwtrf.html

[Q70] 更新统计信息
来源：http://hz.sufxvd.cn/gtxldfvoih.html

ANALYZE TABLE users;
来源：http://hz.vqdsnc.cn/gtzzkwcfin.html

[Q71] 查看建表语句
来源：http://hz.yj20258888.top/gtgawirtqm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sysykeji.top/gtobiymvlz.html

[Q72] 查看索引
来源：http://hz.zhixingplan.top/gtdsjwrjeh.html

SHOW INDEX FROM users;
来源：http://hz.chenjidiqi.icu/gtdibwoxrz.html

[Q73] 查看表状态
来源：http://hz.smart0.xyz/gtjefrjire.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.wangshuangyany.cn/gtmegrunrb.html

[Q74] 强制使用索引
来源：http://hz.gaohongyu789.top/gtywfifxcp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cqqwz.cn/gtziuodklu.html

[Q75] 日期格式化
来源：http://hz.shangyingyoupin.top/gtbrjwflhl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cashguo.top/gtkvznyftt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.iojbl.cn/gtgsfpzwvt.html

[Q76] 按天统计
来源：http://hz.52xcode.cn/gtcezyfssp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.bjfxy.top/gtnvcxpaax.html

[Q77] 时间加减
来源：http://hz.ybcxt.top/gtozergucf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nwbrower.top/gtrpaiiztp.html

[Q78] 当前时间
来源：http://hz.yanxiufei.cn/gtjbkgrqib.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenjidiqi.icu/gtpvkzsalx.html

[Q79] 字符串拼接
来源：http://hz.shangyingyoupin.top/gtsdmygiwm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj20258.top/gtmeijgmfz.html

[Q80] 字符串截取
来源：http://hz.jinqigufen.top/gtzbotnohf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.redwolf501.top/gtgckwukre.html

[Q81] 字符串替换
来源：http://hz.xuetiantiany.cn/gtoogkadqf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gzhubu.top/gtpequjpic.html

[Q82] 字符长度与字节长度
来源：http://hz.9152youxi.cn/gtodbsathk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ppjwa.cn/gtdsdozfzr.html

[Q83] 大小写转换
来源：http://hz.tianlin.xyz/gtlcyflvul.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtzbqguxcs.html

[Q84] 去除首尾空格
来源：http://hz.ydzc1.top/gtjepipsah.html

SELECT TRIM(name) FROM users;
来源：http://hz.birdmap.top/gtqxlaallx.html

[Q85] 数值取整
来源：http://hz.tian-w.cn/gtwydszlzz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.guowangkeji.top/gtvmcppmin.html

[Q86] 读取 JSON 字段
来源：http://hz.hongshengwenyu.top/gtgnwlrpgh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.andypj.xyz/gtokzfxdmh.html

[Q87] JSON 字段做条件
来源：http://hz.yuxming.cn/gtscnzhysz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gotoacloud.top/gtcrdljkxi.html

[Q88] 行转列（条件聚合）
来源：http://hz.sxryk.cn/gtpkhzasdc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.316326.xyz/gtxyaznqfn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.52xcode.cn/gtiaxxxpfp.html

[Q89] 判断表是否存在
来源：http://hz.hywenlv.cn/gtidqvpvze.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.dashuyun.cn/gtrddayrux.html

[Q90] 生成序号列
来源：http://hz.kuanghao11.cn/gtdkchrhtl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.iojbl.cn/gtjlazseae.html

================================================================================
来源：http://hz.gzhubu.top/gtifhbfxiq.html

R. Bash 专题
来源：http://hz.0kj1m.cn/gtwtrcyfsy.html

================================================================================
来源：http://hz.sweek.top/gtizfyeske.html

[R01] shebang 与严格模式
来源：http://hz.jinghuilouyu.cn/gtklilcpid.html

#!/usr/bin/env bash
来源：http://hz.redwolf501.top/gtacryltjs.html

set -euo pipefail
来源：http://hz.nanxuanxn.top/gtasoyaeth.html

[R02] 变量赋值与使用
来源：http://hz.zhaomingkeji.xyz/gtigxtywjy.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gthunhzacy.html

[R03] 只读变量
来源：http://hz.guannengcc.top/gtvnthxvjb.html

readonly PI=3.14
来源：http://hz.shuidangran.top/gtrglxqymc.html

[R04] 位置参数
来源：http://hz.tanke756.top/gtjoppngcf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhaomingkeji.xyz/gtvcjhcbdh.html

[R05] 参数默认值
来源：http://hz.zhengqikj.top/gtpjykvruu.html

name="${1:-default}"
来源：http://hz.9152youxi.cn/gtixrrxmsy.html

[R06] 判断命令是否存在
来源：http://hz.xuetiantiany.cn/gtjedunbbf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fzhhl.top/gtjnzokhya.html

[R07] if 判断文件
来源：http://hz.tanke756.top/gtylhtandd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhongyouzk.top/gtegjpemrw.html

[R08] 数值比较
来源：http://hz.xinyue.icu/gtvburrufk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.svipenyu.cn/gttahuhnzk.html

[R09] 字符串比较
来源：http://hz.jinqigufen.top/gtabtsxcnf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ehwqpu.com/gtxlyciyxx.html

[R10] 正则匹配
来源：http://hz.yanxiufei.cn/gtlswgyfsi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuanzhike.top/gtxtbfloki.html

[R11] case 多分支
来源：http://hz.jiagoushi.top/gtcliapccv.html

case "$1" in
来源：http://hz.52xcode.cn/gtpclaoiwm.html

start) echo "启动" ;;
来源：http://hz.andypj.xyz/gtvyvghwpn.html

stop)  echo "停止" ;;
来源：http://hz.wangshuangyany.cn/gtnqcdrmne.html

*)     echo "未知命令" ;;
来源：http://hz.9152youxi.cn/gtdlpkgmfz.html

esac
来源：http://hz.zhijiandao.cn/gtbffuydsc.html

[R12] for 遍历文件
来源：http://hz.0kj1m.cn/gtsxzeuukh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigufen.top/gtnxhbcrxy.html

[R13] for 计数循环
来源：http://hz.iojbl.cn/gtaphfgoih.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxinkj.top/gteymamtbl.html

[R14] C 风格 for
来源：http://hz.daxiang520.top/gtrcyexzfy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhaomingkeji.xyz/gtxzfoylbk.html

[R15] while 逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtqcsgqgzz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.iojbl.cn/gtxftitxkp.html

[R16] until 等待条件
来源：http://hz.yangfankeji.com/gtpvbmnbmu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.316326.xyz/gtswbkycyd.html

[R17] 数组定义与取值
来源：http://hz.haohaochexian.top/gtenugzbpy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jyoumei.cn/gtvkrxwpyt.html

[R18] 遍历数组
来源：http://hz.sxryk.cn/gtwdsaezro.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangdashe.top/gtiwdboesy.html

[R19] 数组长度
来源：http://hz.yj20258.top/gtdfximzdz.html

echo "${#arr[@]}"
来源：http://hz.jinyuanbaomall.cn/gtyxkewmpx.html

[R20] 关联数组（字典）
来源：http://hz.shanyushiyangtech.top/gtmguysads.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinghuilouyu.cn/gtxgxkauav.html

[R21] 字符串长度
来源：http://hz.xuanzx.com/gtanwmnaku.html

echo "${#s}"
来源：http://hz.hnxiangtu.top/gtxjijmmsk.html

[R22] 截取子串
来源：http://hz.andypj.xyz/gtuegzqsxj.html

echo "${s:0:5}"
来源：http://hz.gzhubu.top/gtyvgmqtev.html

[R23] 字符串替换
来源：http://hz.zhongyouzk.top/gtdatipbad.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.daria6918.cn/gtjhxtdhfu.html

[R24] 大小写转换
来源：http://hz.sweek.top/gtiqhcadcf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hywenlv.cn/gtbuwonuwn.html

[R25] 去后缀 / 去前缀
来源：http://hz.quarkkingdee.top/gtxmopaiwy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xinyue.icu/gtgoilwziz.html

[R26] 命令替换
来源：http://hz.tian-w.cn/gtthbrboye.html

now=$(date +%F); echo "$now"
来源：http://hz.hongshengwenyu.top/gtsjqdrzco.html

[R27] 算术展开
来源：http://hz.sxryk.cn/gtzrqzdfqt.html

echo $((1 + 2 * 3))
来源：http://hz.tanke756.top/gtbvqivyjd.html

[R28] 浮点运算
来源：http://hz.shuidangran.top/gtpydfiqxg.html

echo "scale=2; 10/3" | bc
来源：http://hz.yuxming.cn/gtjrkxixzh.html

[R29] 定义函数
来源：http://hz.jinyuanbaomall.cn/gtxespetua.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jianghu66.top/gtmskwoayj.html

[R30] 函数返回状态码
来源：http://hz.dianchejie.cn/gtdnqwlcho.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhixingplan.top/gtwiikqjyc.html

[R31] 局部变量
来源：http://hz.hongshengwenyu.top/gtdxgsomqd.html

f() { local x=1; echo "$x"; }
来源：http://hz.sweek.top/gtgisyuzam.html

[R32] 参数个数校验
来源：http://hz.pycfn.com/gtcxtrzjhd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.snrcjt.cn/gtayotjskt.html

[R33] 捕获错误并提示行号
来源：http://hz.cashguo.top/gtadjsofbd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zdqjudy.top/gtfljjhxcj.html

[R34] 退出时清理
来源：http://hz.yanxiufei.cn/gtevtoyfxm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gtiqvgztsg.html

[R35] 后台执行并等待
来源：http://hz.xylfe.cn/gtyelxxxtv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.havefunace.top/gtxejpbndf.html

[R36] 并发执行多个任务
来源：http://hz.jiagoushi.top/gtmutunoyu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.vqdsnc.cn/gtmijuapot.html

[R37] 把输出赋给变量
来源：http://hz.redwolf501.top/gtnvxadaoy.html

files=$(ls -1)
来源：http://hz.hammf.cn/gtnrpdycgv.html

[R38] 管道串联
来源：http://hz.jlsjyb.cn/gtegyvzael.html

cat a.txt | grep -i error | wc -l
来源：http://hz.redwolf501.top/gtqznkuzlh.html

[R39] 重定向标准输出与错误
来源：http://hz.yonumen.top/gtlckqdtxj.html

cmd > out.log 2>&1
来源：http://hz.guannengcc.top/gthiofkbip.html

[R40] 追加写日志
来源：http://hz.tianlin.xyz/gtrivcnaxj.html

echo "log" >> out.log
来源：http://hz.pycfn.com/gtljhtqncj.html

[R41] 丢弃输出
来源：http://hz.sysykeji.top/gtjmadnwbs.html

cmd >/dev/null 2>&1
来源：http://hz.chenjidiqi.icu/gtxoqcbeav.html

[R42] 输入重定向
来源：http://hz.shangyingyoupin.top/gtsozedtit.html

wc -l < a.txt
来源：http://hz.xziqi.cn/gtaqcseebb.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtessghnix.html

find . -name "*.log" -type f
来源：http://hz.zhixingplan.top/gtcpnjmqtp.html

[R44] 按修改时间查找
来源：http://hz.316326.xyz/gtztrutiyk.html

find . -mtime -7 -type f
来源：http://hz.zhengqikj.top/gtqbensqjd.html

[R45] 批量删除
来源：http://hz.gaohongyu789.top/gtafpqqeqy.html

find . -name "*.tmp" -delete
来源：http://hz.wangshuangyany.cn/gtnymspkfk.html

[R46] 递归替换文件内容
来源：http://hz.vqdsnc.cn/gtszqfxqrb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.aibaodan.cn/gtxvgegimo.html

[R47] sed 单行替换
来源：http://hz.fzhhl.top/gteylwdprp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xylfe.cn/gtvvjaibnh.html

[R48] awk 取指定列
来源：http://hz.sweek.top/gtnmuqtmxm.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhijiandao.cn/gtjrzxohcb.html

[R49] awk 带条件
来源：http://hz.hongshengwenyu.top/gtlrevdhdr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.quarkkingdee.top/gtrzllutth.html

[R50] awk 求和
来源：http://hz.pengpengdd.cyou/gtvuqczmat.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hfpthk.cn/gtsifrmxgn.html

[R51] 排序去重取前几
来源：http://hz.bjfxy.top/gtcvzeikeh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.meibo888.top/gtwgcyehvh.html

[R52] 统计行数
来源：http://hz.fengsongda.top/gtdagticoq.html

wc -l a.txt
来源：http://hz.zhaomingkeji.xyz/gtsmcwgqlz.html

[R53] 查看文件头与实时尾
来源：http://hz.nanxuanxn.top/gtiqffitku.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aizwys.cn/gtxvucgvjj.html

[R54] 比较两个文件
来源：http://hz.sweek.top/gtlntpnrty.html

diff a.txt b.txt
来源：http://hz.wangdashe.top/gtpbtumbvz.html

[R55] 压缩与解压
来源：http://hz.xylfe.cn/gthlicitcu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shanyushiyangkeji.top/gtduithbcq.html

[R56] 远程拷贝
来源：http://hz.vqdsnc.cn/gttwwhuhyk.html

scp file user@host:/path/
来源：http://hz.ydzc1.top/gtlktarqmd.html

[R57] 远程执行命令
来源：http://hz.andypj.xyz/gtzcunhgeh.html

ssh user@host 'uptime'
来源：http://hz.hnqzz.top/gtrezxbmqc.html

[R58] 下载文件
来源：http://hz.aizwys.cn/gtchhfyaev.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.vqdsnc.cn/gtogiagvao.html

[R59] 发 POST JSON
来源：http://hz.yvedp.cn/gttyjgccnh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydjk.org.cn/gtbeoimvyf.html

[R60] 只看 HTTP 状态码
来源：http://hz.meibo888.top/gtfbaxbmpq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tianlin.xyz/gtlvojbxwm.html

[R61] 磁盘占用
来源：http://hz.svipenyu.cn/gtnsieuqii.html

df -h;  du -sh *
来源：http://hz.yanxiufei.cn/gtgokfcvwr.html

[R62] 找最占空间的文件
来源：http://hz.havefunace.top/gtvxvbqhrp.html

du -ah . | sort -rh | head -10
来源：http://hz.haohaochexian.top/gtzqyrksnp.html

[R63] 内存与进程
来源：http://hz.tanke756.top/gthccefdtl.html

free -h;  ps aux | grep nginx
来源：http://hz.ydjk.org.cn/gtmkuhqqab.html

[R64] 结束进程
来源：http://hz.yuanzhike.top/gtbnxobraz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cashguo.top/gtbpqyaecf.html

[R65] 查看端口占用
来源：http://hz.yj20258888.top/gtwyyfzfkv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj20258888.top/gtckdvimcw.html

[R66] 定时任务
来源：http://hz.smart0.xyz/gthzkswxiq.html

crontab -e;  crontab -l
来源：http://hz.jinqigufen.top/gtcdheuign.html

[R67] 生成随机十六进制串
来源：http://hz.hnxiangtu.top/gthrxkpxby.html

openssl rand -hex 16
来源：http://hz.dashuyun.cn/gtdldtjkcw.html

[R68] 计算文件校验值
来源：http://hz.shzxlz.cn/gthfuxhccy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jiagoushi.top/gtajjtowdg.html

[R69] 生成随机密码
来源：http://hz.shangyingyoupin.top/gtbzghzimw.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhiwuduotai.top/gteroxshbv.html

[R70] 时间戳与互转
来源：http://hz.smart0.xyz/gtbosliqmr.html

date +%s;  date -d @1700000000
来源：http://hz.jianghu66.top/gtirdacqvp.html

[R71] 日期格式化
来源：http://hz.gotoacloud.top/gtivprcxax.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.daria6918.cn/gtzdmvfnvq.html

[R72] 等待端口就绪
来源：http://hz.jinqigfzy.top/gtpheghdtn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jqgufenzy.top/gtexasyeao.html

[R73] 分割大日志
来源：http://hz.sufxvd.cn/gtefhcsvhs.html

split -l 1000 big.log part_
来源：http://hz.feifeiyinyue.top/gtayxteyvt.html

[R74] 批量重命名
来源：http://hz.yuanzhike.top/gtrvtvugik.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.feifeiyinyue.top/gtyxllrfns.html

[R75] 导出环境变量
来源：http://hz.yuanzhike.top/gtuzqtsidw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yueranfly.top/gtpvgwcwxg.html

[R76] 使用临时文件
来源：http://hz.zhaomingkeji.xyz/gtihkoatbx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gaohongyu789.top/gtkhuvkjhi.html

[R77] 读取用户输入
来源：http://hz.cheryme.top/gtihosjgek.html

read -rp "请输入: " ans
来源：http://hz.cashguo.top/gtbustbhlb.html

[R78] 交互式菜单
来源：http://hz.pycfn.com/gtovxfgkjt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tian-w.cn/gtjmmhnnor.html

[R79] 解析命令行选项
来源：http://hz.pengpengdd.cyou/gtmtjanwwk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sweek.top/gtisapirov.html

[R80] 查看脚本执行耗时
来源：http://hz.jinghuilouyu.cn/gtartqqqvc.html

time ./run.sh
来源：http://hz.shuidangran.top/gtrqnndqgu.html

================================================================================
来源：http://hz.mhx1999.top/gtazlkmydc.html

S. C / C++ 专题
来源：http://hz.jqgfzy.top/gtbfoemeln.html

================================================================================
来源：http://hz.jlsjyb.cn/gtdfanlqvh.html

[S01] C：Hello World
来源：http://hz.cucudq.cn/gthmfbdlqm.html

#include <stdio.h>
来源：http://hz.ywan-chungtsiang.top/gtzleclkfh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.snrcjt.cn/gtvitanzfj.html

[S02] C：变量与格式化输出
来源：http://hz.wangdashe.top/gtywwenetp.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhengqikj.top/gtzmpwtlcc.html

[S03] C：读入整数
来源：http://hz.ydjk.org.cn/gtvvzfympg.html

int x; scanf("%d", &x);
来源：http://hz.svipenyu.cn/gtqtueoynr.html

[S04] C：字符串复制
来源：http://hz.redwolf501.top/gtmdupbfhe.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.guowangkeji.top/gthjzqfalu.html

[S05] C：字符串长度
来源：http://hz.zycfv.cn/gtcegxonzu.html

strlen(s)
来源：http://hz.cdnleiting.top/gtlxhxodqo.html

[S06] C：字符串比较
来源：http://hz.yangfankeji.com/gtmzflcase.html

strcmp(a, b) == 0
来源：http://hz.zycfv.cn/gtvrkkhdyl.html

[S07] C：数组遍历求和
来源：http://hz.ybcxt.top/gtytrtkdzo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.vqdsnc.cn/gtfhjdnhox.html

[S08] C：动态内存分配与释放
来源：http://hz.9152youxi.cn/gtshkdclsk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.wangshuangyany.cn/gtdettuluu.html

[S09] C：结构体定义与初始化
来源：http://hz.bjfxy.top/gtgyhhjegp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dianchejie.cn/gtopslkiqd.html

[S10] C：指针与解引用
来源：http://hz.wangdashe.top/gtbqjwycww.html

int *p = &a;  *p = 5;
来源：http://hz.jyoumei.cn/gtacmrvtkg.html

[S11] C：逐行读文件
来源：http://hz.yueranfly.top/gtfuwztcvs.html


<!-- 参考信息 -->