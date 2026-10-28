代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhiwuduotai.top/gtctjhcgao.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yongpay.top/gtchztbcmt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cqqwz.cn/gtdhqrdjvq.html

[Q42] 连接条件附加过滤
来源：http://hz.c1oappe.top/gtrvxkldke.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinyuanbaomall.cn/gtcuuokfbu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.meibo888.top/gtccymropl.html

[Q43] 标量子查询
来源：http://hz.fzhhl.top/gtmrhgwehh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sysykeji.top/gtlrsysfxj.html

[Q44] IN 子查询
来源：http://hz.svipenyu.cn/gthfwchhmy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ybcxt.top/gtmesbztcp.html

[Q45] EXISTS 判断存在
来源：http://hz.xziqi.cn/gtnulmdwgk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuxming.cn/gtfclfsicw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gzhubu.top/gthtjvahvj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangdashe.top/gtgksnslob.html

[Q47] 与平均值比较
来源：http://hz.c1oappe.top/gtovjbfhxc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxinkj.top/gttvbnwzhq.html

[Q48] CTE 公用表表达式
来源：http://hz.52xcode.cn/gtasvjzofx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.316326.xyz/gtqsgscykd.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhixingplan.top/gtfufsntkv.html

[Q49] 更新单行
来源：http://hz.yvedp.cn/gtbhutwktt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinqigufen.top/gtzenptjyn.html

[Q50] 批量更新
来源：http://hz.shangyingyoupin.top/gtgpmbghea.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenzaomai.com/gtcixgdbhb.html

[Q51] 用子查询更新
来源：http://hz.snrcjt.cn/gtopwixthg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yongpay.top/gtinhlrzxn.html

[Q52] 删除指定行
来源：http://hz.hysaishi.cn/gtwsfjndkd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj20258888.top/gtzpebqbmq.html

[Q53] 按条件删除
来源：http://hz.shzxlz.cn/gtnhzotbdc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj20258.top/gtcbhskjdt.html

[Q54] 清空表
来源：http://hz.hfpthk.cn/gtwqzxbmdf.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258888.top/gtptzbrooh.html

[Q55] 排名（并列占位）
来源：http://hz.havefunace.top/gtnvjionym.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cdnleiting.top/gtkbtfiiqp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgfzy.top/gtnigkdazq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.redwolf501.top/gtkcxquttr.html

[Q57] 行号
来源：http://hz.nanxinkj.top/gtbahfogca.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.tian-w.cn/gtpjiariim.html

[Q58] 累计求和
来源：http://hz.jqgfzy.top/gteueshevx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xuanzx.com/gtdjmazcik.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangtech.top/gtdfnttsll.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tanke756.top/gtlcbvvdxw.html

[Q60] 取上一行 / 下一行
来源：http://hz.nanxinkj.top/gtbanqzfca.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangshuangyany.cn/gtraxdmkfp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pycfn.com/gtwinfxilt.html

[Q61] 移动平均
来源：http://hz.shanyushiyangkeji.top/gtmupofcvv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xziqi.cn/gtmktmefrs.html

[Q62] 分组占比
来源：http://hz.nanxuanxn.top/gtwwyvccgr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtqvyuhphz.html

[Q63] 开启事务
来源：http://hz.jinghuilouyu.cn/gtxwcxxnai.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tian-w.cn/gtnwwocuba.html

[Q64] 提交事务
来源：http://hz.zhijiandao.cn/gttbvzjgog.html

COMMIT;
来源：http://hz.xuanzx.com/gtupfysoog.html

[Q65] 回滚事务
来源：http://hz.iojbl.cn/gtzysckpqa.html

ROLLBACK;
来源：http://hz.yuxming.cn/gtufspiwcm.html

[Q66] 行锁查询
来源：http://hz.chenzaomai.com/gtzxaadqzq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pengpengdd.cyou/gtwywgbtln.html

[Q67] 设置隔离级别
来源：http://hz.ydzc1.top/gtiyiklboc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hywenlv.cn/gtvegarkmi.html

[Q68] 保存点
来源：http://hz.jqgufenzy.top/gtyotibfnj.html

SAVEPOINT sp1;
来源：http://hz.fengsongda.top/gtzctryxfj.html

ROLLBACK TO sp1;
来源：http://hz.cqqwz.cn/gtvpqzbhkr.html

[Q69] 查看执行计划
来源：http://hz.quarkkingdee.top/gtmlkrqkvd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.pycfn.com/gtcgmrlzxh.html

[Q70] 更新统计信息
来源：http://hz.cheryme.top/gtmnnxhtif.html

ANALYZE TABLE users;
来源：http://hz.shanyushiyangkeji.top/gtydgzzedy.html

[Q71] 查看建表语句
来源：http://hz.shangyingyoupin.top/gtaokodqhg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jlsjyb.cn/gtoyzcsvqe.html

[Q72] 查看索引
来源：http://hz.yvedp.cn/gtgbzdkmrv.html

SHOW INDEX FROM users;
来源：http://hz.zhengqikj.top/gtyxyssdlw.html

[Q73] 查看表状态
来源：http://hz.shanyushiyangkeji.top/gtjmgsapfv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinqigufen.top/gtlsmemema.html

[Q74] 强制使用索引
来源：http://hz.pycfn.com/gtuzewvtnd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cqqwz.cn/gtqfcaqlnm.html

[Q75] 日期格式化
来源：http://hz.jiagoushi.top/gtikgjagai.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xylfe.cn/gtfhomhihu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xuanzx.com/gtdvgeqwbl.html

[Q76] 按天统计
来源：http://hz.fzhhl.top/gttyjtylev.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.mhx1999.top/gtyqcmdbzg.html

[Q77] 时间加减
来源：http://hz.xuetiantiany.cn/gthfygduaa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.daxiang520.top/gtltsoihca.html

[Q78] 当前时间
来源：http://hz.zhoulong.xyz/gtvwfxbyld.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ydjk.org.cn/gtuyrvdrgq.html

[Q79] 字符串拼接
来源：http://hz.shuidangran.top/gtuondoakm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ehwqpu.com/gtclkgxbnf.html

[Q80] 字符串截取
来源：http://hz.hnxiangtu.top/gtgqpaxmaa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cucudq.cn/gtykcyuyfz.html

[Q81] 字符串替换
来源：http://hz.jinghuilouyu.cn/gtxezcpqff.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.birdmap.top/gtcyqtthbt.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxuanxn.top/gtsyiezmxd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.52xcode.cn/gtinwzlnmo.html

[Q83] 大小写转换
来源：http://hz.yonumen.top/gtuxxjwmbx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ydjk.org.cn/gtahfvzwxj.html

[Q84] 去除首尾空格
来源：http://hz.guannengcc.top/gtfgpgqdmv.html

SELECT TRIM(name) FROM users;
来源：http://hz.iojbl.cn/gtmrlkvqok.html

[Q85] 数值取整
来源：http://hz.zhongyouzk.top/gthuzdiemd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cqqwz.cn/gtfwgpezab.html

[Q86] 读取 JSON 字段
来源：http://hz.nwbrower.top/gtggdeqcpx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinqigufen.top/gthnfsxbwk.html

[Q87] JSON 字段做条件
来源：http://hz.nwbrower.top/gtfanabtyt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sxryk.cn/gtkllumtig.html

[Q88] 行转列（条件聚合）
来源：http://hz.xylfe.cn/gtfhjmxvur.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigfzy.top/gtnwinzsff.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.dianchejie.cn/gthpjglqul.html

[Q89] 判断表是否存在
来源：http://hz.52xcode.cn/gtkzsfbxas.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hammf.cn/gtgfjnqthc.html

[Q90] 生成序号列
来源：http://hz.aizwys.cn/gtnwrmvhwx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yueranfly.top/gtzdnzgqeb.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtcdejvqpp.html

R. Bash 专题
来源：http://hz.cdnleiting.top/gtrpgnzfmm.html

================================================================================
来源：http://hz.yanxiufei.cn/gtgctdubxi.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangkeji.top/gtofjfgoyw.html

#!/usr/bin/env bash
来源：http://hz.jinqigufen.top/gtcebndsnw.html

set -euo pipefail
来源：http://hz.mhx1999.top/gtovgeldmb.html

[R02] 变量赋值与使用
来源：http://hz.gaohongyu789.top/gttdfzqnzw.html

name="Tom"; echo "$name"
来源：http://hz.nanxinkj.top/gtkmcuqcdw.html

[R03] 只读变量
来源：http://hz.hnxiangtu.top/gtgmfvahgp.html

readonly PI=3.14
来源：http://hz.meibo888.top/gtglepqxiz.html

[R04] 位置参数
来源：http://hz.sysykeji.top/gtnsabbvkc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.andypj.xyz/gtzeapbgcm.html

[R05] 参数默认值
来源：http://hz.hfpthk.cn/gtpxlrvbim.html

name="${1:-default}"
来源：http://hz.sufxvd.cn/gtvspvfadc.html

[R06] 判断命令是否存在
来源：http://hz.zhixingplan.top/gtyzqoitoy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.bjfxy.top/gtnapfspva.html

[R07] if 判断文件
来源：http://hz.yangfankeji.com/gtmarxgaak.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ywan-chungtsiang.top/gtfclwdiwv.html

[R08] 数值比较
来源：http://hz.cheryme.top/gtnchnfngw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.fengsongda.top/gtxpufciuh.html

[R09] 字符串比较
来源：http://hz.c1oappe.top/gtluahbipm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yangfankeji.com/gtuakewpyk.html

[R10] 正则匹配
来源：http://hz.dianchejie.cn/gtikfftdaa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.birdmap.top/gtyaydpgsa.html

[R11] case 多分支
来源：http://hz.yj20258888.top/gtfvqonnox.html

case "$1" in
来源：http://hz.sxryk.cn/gtkxklsaxi.html

start) echo "启动" ;;
来源：http://hz.hywenlv.cn/gtkdtqlcjn.html

stop)  echo "停止" ;;
来源：http://hz.52xcode.cn/gtprslqtnm.html

*)     echo "未知命令" ;;
来源：http://hz.52xcode.cn/gtfrjzsimq.html

esac
来源：http://hz.hysaishi.cn/gtobnoopbf.html

[R12] for 遍历文件
来源：http://hz.yueranfly.top/gtlivvrmvs.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xingfuxueyuan.xyz/gtfgntbncs.html

[R13] for 计数循环
来源：http://hz.chenlongwang.top/gtdwyjfcvq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xinyue.icu/gtfwpgunmo.html

[R14] C 风格 for
来源：http://hz.jiagoushi.top/gtqtwhnwum.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.wangshuangyany.cn/gtnqgnafgs.html

[R15] while 逐行读文件
来源：http://hz.ehwqpu.com/gtnqeuowhm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yonumen.top/gtpehosoux.html

[R16] until 等待条件
来源：http://hz.tanke756.top/gttceapmqi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtrxjmrewa.html

[R17] 数组定义与取值
来源：http://hz.sysykeji.top/gttthahuaw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.vqdsnc.cn/gtmmgrgjqi.html

[R18] 遍历数组
来源：http://hz.sysykeji.top/gtekulvcky.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.nanxinkj.top/gtndnnwovo.html

[R19] 数组长度
来源：http://hz.xziqi.cn/gturyhlyxx.html

echo "${#arr[@]}"
来源：http://hz.zhijiandao.cn/gtalhswnhs.html

[R20] 关联数组（字典）
来源：http://hz.jinqigfzy.top/gtikzjmkdf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.9152youxi.cn/gtmhmtldta.html

[R21] 字符串长度
来源：http://hz.fengsongda.top/gtsmvpxrzl.html

echo "${#s}"
来源：http://hz.aizwys.cn/gtrrxfonbv.html

[R22] 截取子串
来源：http://hz.hysaishi.cn/gtagdzjmgf.html

echo "${s:0:5}"
来源：http://hz.guowangkeji.top/gtlgyhyluv.html

[R23] 字符串替换
来源：http://hz.yongpay.top/gtcactymii.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj202588.top/gthiwtucrs.html

[R24] 大小写转换
来源：http://hz.gogol.net.cn/gtsuqvelau.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hammf.cn/gthdlcizij.html

[R25] 去后缀 / 去前缀
来源：http://hz.jianghu66.top/gtlhzifehl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ppjwa.cn/gtcrhrmqsl.html

[R26] 命令替换
来源：http://hz.ydzc1.top/gtwkpsseze.html

now=$(date +%F); echo "$now"
来源：http://hz.aizwys.cn/gtjwiksamv.html

[R27] 算术展开
来源：http://hz.zycfv.cn/gtdlnsszdo.html

echo $((1 + 2 * 3))
来源：http://hz.guannengcc.top/gtygbxxpzu.html

[R28] 浮点运算
来源：http://hz.pengpengdd.cyou/gtqosyeldk.html

echo "scale=2; 10/3" | bc
来源：http://hz.gogol.net.cn/gtdbbtgnap.html

[R29] 定义函数
来源：http://hz.redwolf501.top/gtgbchssnt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.birdmap.top/gtlqdqgczi.html

[R30] 函数返回状态码
来源：http://hz.havefunace.top/gtksfwwift.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.iojbl.cn/gtivfdxmrx.html

[R31] 局部变量
来源：http://hz.sxryk.cn/gtwfxfpqvs.html

f() { local x=1; echo "$x"; }
来源：http://hz.zdqjudy.top/gtwkbgilkf.html

[R32] 参数个数校验
来源：http://hz.dianchejie.cn/gtkemmbnqz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.andypj.xyz/gtnmpdvbzo.html

[R33] 捕获错误并提示行号
来源：http://hz.xingfuxueyuan.xyz/gtgokvwwed.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.bjfxy.top/gtokvtkbtn.html

[R34] 退出时清理
来源：http://hz.jianghu66.top/gtjqyimxkn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258888.top/gtfesxooaw.html

[R35] 后台执行并等待
来源：http://hz.vqdsnc.cn/gtmiyuyxdf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.iojbl.cn/gtzeltsnmd.html

[R36] 并发执行多个任务
来源：http://hz.nanxinkj.top/gttpxwbpls.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cheryme.top/gtsijenllk.html

[R37] 把输出赋给变量
来源：http://hz.chenjidiqi.icu/gtymjgfaga.html

files=$(ls -1)
来源：http://hz.jqgufenzy.top/gtvqbywflm.html

[R38] 管道串联
来源：http://hz.jinqigfzy.top/gtqmqdftes.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhengqikj.top/gtqvefinqw.html

[R39] 重定向标准输出与错误
来源：http://hz.dianchejie.cn/gtjooedgeq.html

cmd > out.log 2>&1
来源：http://hz.0kj1m.cn/gthgtfvzfd.html

[R40] 追加写日志
来源：http://hz.hnqzz.top/gtevhcfgqc.html

echo "log" >> out.log
来源：http://hz.hywenlv.cn/gtxvxofuhw.html

[R41] 丢弃输出
来源：http://hz.hysaishi.cn/gtwhatyfhp.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangtech.top/gttvhpgbmc.html

[R42] 输入重定向
来源：http://hz.cqqwz.cn/gtaxbmjnck.html

wc -l < a.txt
来源：http://hz.cashguo.top/gtqhywlzcl.html

[R43] 按名字查找文件
来源：http://hz.dashuyun.cn/gtxsotznpj.html

find . -name "*.log" -type f
来源：http://hz.yangfankeji.com/gtrijjcwyj.html

[R44] 按修改时间查找
来源：http://hz.wangshuangyany.cn/gttpfrzyqa.html

find . -mtime -7 -type f
来源：http://hz.c1oappe.top/gtcpnoxnpi.html

[R45] 批量删除
来源：http://hz.redwolf501.top/gtmgoxbhpv.html

find . -name "*.tmp" -delete
来源：http://hz.shangyingyoupin.top/gtzmhnnmwy.html

[R46] 递归替换文件内容
来源：http://hz.cdnleiting.top/gtzmkkksxz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shuidangran.top/gttuqqnetw.html

[R47] sed 单行替换
来源：http://hz.guannengcc.top/gtqnjskzxx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenjidiqi.icu/gtkhksnloq.html

[R48] awk 取指定列
来源：http://hz.ydjk.org.cn/gtmaozjoka.html

awk '{print $1, $3}' a.txt
来源：http://hz.cucudq.cn/gthnlugqui.html

[R49] awk 带条件
来源：http://hz.hysaishi.cn/gtfkiitbnd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gogol.net.cn/gtoojhfqdl.html

[R50] awk 求和
来源：http://hz.jiagoushi.top/gtshcrbakf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cqqwz.cn/gtabokhxql.html

[R51] 排序去重取前几
来源：http://hz.sufxvd.cn/gtrbhbbusk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sufxvd.cn/gtndavglwp.html

[R52] 统计行数
来源：http://hz.shanyushiyangkeji.top/gtjkjelcvf.html

wc -l a.txt
来源：http://hz.gzhubu.top/gtjxdhzbnr.html

[R53] 查看文件头与实时尾
来源：http://hz.zhengqikj.top/gtlavsvalk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.iojbl.cn/gtgmhittiv.html

[R54] 比较两个文件
来源：http://hz.gogol.net.cn/gtsbpeedoe.html

diff a.txt b.txt
来源：http://hz.jinqigfzy.top/gtfspevjvl.html

[R55] 压缩与解压
来源：http://hz.feifeiyinyue.top/gteygmsvba.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gogol.net.cn/gtbheljdan.html

[R56] 远程拷贝
来源：http://hz.yanxiufei.cn/gtpmhwtqsc.html

scp file user@host:/path/
来源：http://hz.tian-w.cn/gtmenvaigg.html

[R57] 远程执行命令
来源：http://hz.smart0.xyz/gtqsyddxhm.html

ssh user@host 'uptime'
来源：http://hz.zhengqikj.top/gtpddnxyqk.html

[R58] 下载文件
来源：http://hz.jqgfzy.top/gtqetlhctl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.kuanghao11.cn/gtfyjxrygr.html

[R59] 发 POST JSON
来源：http://hz.cheryme.top/gtmymlqbsm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.52xcode.cn/gtigmiwjrd.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtgvcpvyrw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinyuanbaomall.cn/gtthbeuezq.html

[R61] 磁盘占用
来源：http://hz.smart0.xyz/gthuyihfwo.html

df -h;  du -sh *
来源：http://hz.tanke756.top/gtitkvbhxc.html

[R62] 找最占空间的文件
来源：http://hz.yongpay.top/gtqfensbpy.html

du -ah . | sort -rh | head -10
来源：http://hz.pycfn.com/gtocwvhsud.html

[R63] 内存与进程
来源：http://hz.feifeiyinyue.top/gtqnmekffs.html

free -h;  ps aux | grep nginx
来源：http://hz.kuanghao11.cn/gtqkmavtbx.html

[R64] 结束进程
来源：http://hz.svipenyu.cn/gtdrpmjfpl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.feifeiyinyue.top/gtwzjhnhzs.html

[R65] 查看端口占用
来源：http://hz.birdmap.top/gtckzshinh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yanxiufei.cn/gtnqopfuvy.html

[R66] 定时任务
来源：http://hz.ppjwa.cn/gtzqbxzljt.html

crontab -e;  crontab -l
来源：http://hz.jyoumei.cn/gtbigqthun.html

[R67] 生成随机十六进制串
来源：http://hz.nwbrower.top/gtmvixzgwe.html

openssl rand -hex 16
来源：http://hz.yj20258888.top/gtinpjbazy.html

[R68] 计算文件校验值
来源：http://hz.meibo888.top/gtontiovlz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dashuyun.cn/gttowelosn.html

[R69] 生成随机密码
来源：http://hz.yanxiufei.cn/gtxzcqjqnk.html

head -c 16 /dev/urandom | base64
来源：http://hz.quarkkingdee.top/gtggmiledn.html

[R70] 时间戳与互转
来源：http://hz.kuanghao11.cn/gtmmizqbsr.html

date +%s;  date -d @1700000000
来源：http://hz.snrcjt.cn/gtfjikiafz.html

[R71] 日期格式化
来源：http://hz.aibaodan.cn/gtxevjwhkk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cqqwz.cn/gtolzojrlp.html

[R72] 等待端口就绪
来源：http://hz.yueranfly.top/gtqkudpbhm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtonvpndyd.html

[R73] 分割大日志
来源：http://hz.vqdsnc.cn/gtxvrrbzdf.html

split -l 1000 big.log part_
来源：http://hz.ywan-chungtsiang.top/gtwionyquz.html

[R74] 批量重命名
来源：http://hz.xziqi.cn/gtfeeeapxk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ehwqpu.com/gtlonfeosg.html

[R75] 导出环境变量
来源：http://hz.zhengqikj.top/gtlmpzbovh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.0kj1m.cn/gtiufdudfc.html

[R76] 使用临时文件
来源：http://hz.tianlin.xyz/gtqktxzbsw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtnrnegnic.html

[R77] 读取用户输入
来源：http://hz.gotoacloud.top/gtzmvsuzir.html

read -rp "请输入: " ans
来源：http://hz.jinghuilouyu.cn/gttetvljmc.html

[R78] 交互式菜单
来源：http://hz.cheryme.top/gtgvazwvbi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jqgfzy.top/gtuwpgzphf.html

[R79] 解析命令行选项
来源：http://hz.chenzaomai.com/gtcsculsdo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.0kj1m.cn/gttwbppylj.html

[R80] 查看脚本执行耗时
来源：http://hz.jinghuilouyu.cn/gtttxxbjcb.html

time ./run.sh
来源：http://hz.sufxvd.cn/gtayyvtbeh.html

================================================================================
来源：http://hz.zhengqikj.top/gtglhezvaw.html

S. C / C++ 专题
来源：http://hz.aibaodan.cn/gtvbtqyqre.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtvmkednog.html

[S01] C：Hello World
来源：http://hz.jlsjyb.cn/gtnsxfllzy.html

#include <stdio.h>
来源：http://hz.cashguo.top/gtlokbacsy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.bjfxy.top/gthyuwxjcz.html

[S02] C：变量与格式化输出
来源：http://hz.yj202588.top/gtqxziyayu.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinyuanbaomall.cn/gtupgqszxn.html

[S03] C：读入整数
来源：http://hz.yueranfly.top/gtgfvuycpf.html

int x; scanf("%d", &x);
来源：http://hz.aizwys.cn/gtgecgodji.html

[S04] C：字符串复制
来源：http://hz.zdqjudy.top/gtszgzodbx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nwbrower.top/gtptmoifma.html

[S05] C：字符串长度
来源：http://hz.shzxlz.cn/gtrjrcnnyn.html

strlen(s)
来源：http://hz.yueranfly.top/gttsrojdoh.html

[S06] C：字符串比较
来源：http://hz.nwbrower.top/gtljrnwamy.html

strcmp(a, b) == 0
来源：http://hz.c1oappe.top/gtuomrvnmr.html

[S07] C：数组遍历求和
来源：http://hz.yvedp.cn/gtndjodxgo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cqqwz.cn/gtksvsgagr.html

[S08] C：动态内存分配与释放
来源：http://hz.zhongyouzk.top/gtglklyjhc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zycfv.cn/gtvkyvcxql.html

[S09] C：结构体定义与初始化
来源：http://hz.gzhubu.top/gtlsxddzhv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xingfuxueyuan.xyz/gtpxkpimks.html

[S10] C：指针与解引用
来源：http://hz.snrcjt.cn/gtiqzsruuy.html

int *p = &a;  *p = 5;
来源：http://hz.zdqjudy.top/gtdkwjgfxd.html

[S11] C：逐行读文件
来源：http://hz.yuxming.cn/gtahhzzppk.html


<!-- 参考信息 -->