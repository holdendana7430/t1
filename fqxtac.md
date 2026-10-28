代发 wailian999

[Q44] IN 子查询
来源：http://hz.ehwqpu.com/gtavvnnkfw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ybcxt.top/gtpzhdjvqi.html

[Q45] EXISTS 判断存在
来源：http://hz.ivvv.top/gteejesqzx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hongshengwenyu.top/gtjgeozhrx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cdnleiting.top/gtlasjdahg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtwkwxccix.html

[Q47] 与平均值比较
来源：http://hz.ydzc1.top/gtpaxvkuuq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhijiandao.cn/gtskijbrvy.html

[Q48] CTE 公用表表达式
来源：http://hz.ivvv.top/gtmyrtmbsz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xziqi.cn/gtmofnkfbh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cdnleiting.top/gtxggwiwqr.html

[Q49] 更新单行
来源：http://hz.nanxuanxn.top/gtjwjnismu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aibaodan.cn/gtvqepbqdf.html

[Q50] 批量更新
来源：http://hz.bjfxy.top/gtxebsfgpw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nwbrower.top/gtfegvslef.html

[Q51] 用子查询更新
来源：http://hz.sweek.top/gtwbeyhutm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ivvv.top/gtjiijgqcg.html

[Q52] 删除指定行
来源：http://hz.cheryme.top/gtipqqktmz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.aizwys.cn/gtzjzmurye.html

[Q53] 按条件删除
来源：http://hz.xuetiantiany.cn/gtxqofuslw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jiagoushi.top/gtqottvdis.html

[Q54] 清空表
来源：http://hz.ehwqpu.com/gtkjcvyhpl.html

TRUNCATE TABLE logs;
来源：http://hz.haohaochexian.top/gtgvumwnqo.html

[Q55] 排名（并列占位）
来源：http://hz.cucudq.cn/gtcnbagjag.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hysaishi.cn/gtktkyykwu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhaomingkeji.xyz/gtubiyggzk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.daxiang520.top/gtnyqhalwe.html

[Q57] 行号
来源：http://hz.iojbl.cn/gtmbkgszpk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sweek.top/gtuideipkw.html

[Q58] 累计求和
来源：http://hz.9152youxi.cn/gtmgawlvuv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.kuanghao11.cn/gtbbzjiead.html

[Q59] 分组内累计
来源：http://hz.cdnleiting.top/gtrykaecnv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cashguo.top/gtnwmwccsx.html

[Q60] 取上一行 / 下一行
来源：http://hz.quarkkingdee.top/gtrqzqrxeb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yueranfly.top/gtmnpqfccx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenzaomai.com/gtjkkttcyq.html

[Q61] 移动平均
来源：http://hz.tanke756.top/gtdpdlbndk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cashguo.top/gtjcdpxyil.html

[Q62] 分组占比
来源：http://hz.jiagoushi.top/gtbhlgtzby.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtrahmrssv.html

[Q63] 开启事务
来源：http://hz.daria6918.cn/gtmnwclwbl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xuetiantiany.cn/gtngahapkh.html

[Q64] 提交事务
来源：http://hz.fengsongda.top/gtrrkotzqo.html

COMMIT;
来源：http://hz.fzhhl.top/gtsfnwnkrc.html

[Q65] 回滚事务
来源：http://hz.jyoumei.cn/gtvrlwgzld.html

ROLLBACK;
来源：http://hz.hnqzz.top/gtnonrarrx.html

[Q66] 行锁查询
来源：http://hz.zhixingplan.top/gtzpytdbll.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sysykeji.top/gtjvebfgnb.html

[Q67] 设置隔离级别
来源：http://hz.chenlongwang.top/gtdtetsyha.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinyuanbaomall.cn/gtpsujveoy.html

[Q68] 保存点
来源：http://hz.zhijiandao.cn/gtzmabakoq.html

SAVEPOINT sp1;
来源：http://hz.cdnleiting.top/gtjtyvhhwh.html

ROLLBACK TO sp1;
来源：http://hz.ydjk.org.cn/gtfssxufyv.html

[Q69] 查看执行计划
来源：http://hz.yj20258888.top/gtutyyixze.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nanxuanxn.top/gtmtpnhmfi.html

[Q70] 更新统计信息
来源：http://hz.pengpengdd.cyou/gtjtsjktlv.html

ANALYZE TABLE users;
来源：http://hz.shangyingyoupin.top/gthfivjvsf.html

[Q71] 查看建表语句
来源：http://hz.ybcxt.top/gtihnssyii.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ydzc1.top/gtstphyqam.html

[Q72] 查看索引
来源：http://hz.guannengcc.top/gtfzatlcsi.html

SHOW INDEX FROM users;
来源：http://hz.jlsjyb.cn/gtzravptvz.html

[Q73] 查看表状态
来源：http://hz.yueranfly.top/gtkxlqdren.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hysaishi.cn/gtupdlzxtw.html

[Q74] 强制使用索引
来源：http://hz.nanxinkj.top/gtbhhzubvn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jlsjyb.cn/gtvxdqgmoq.html

[Q75] 日期格式化
来源：http://hz.yuanzhike.top/gtnvddimyr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yvedp.cn/gtnvofidzf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.andypj.xyz/gtlwqyqvir.html

[Q76] 按天统计
来源：http://hz.gaohongyu789.top/gtvitowjwj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ivvv.top/gtrtpqlwtx.html

[Q77] 时间加减
来源：http://hz.nwbrower.top/gtpeljibgx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yongpay.top/gtbssrxjxq.html

[Q78] 当前时间
来源：http://hz.yangfankeji.com/gtftuwzqaw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jqgufenzy.top/gtbriqeffu.html

[Q79] 字符串拼接
来源：http://hz.sysykeji.top/gtxpfgynbj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xinyue.icu/gtfcewtjyw.html

[Q80] 字符串截取
来源：http://hz.yueranfly.top/gtwviyxsnd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtmsdedxko.html

[Q81] 字符串替换
来源：http://hz.shuidangran.top/gtjreknspp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnqzz.top/gtmnobbhdr.html

[Q82] 字符长度与字节长度
来源：http://hz.dashuyun.cn/gterczsvtc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.quarkkingdee.top/gthpspqaiq.html

[Q83] 大小写转换
来源：http://hz.yonumen.top/gtxhzcyrzw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cdnleiting.top/gtahehdbgu.html

[Q84] 去除首尾空格
来源：http://hz.shuidangran.top/gtgnqvwhxh.html

SELECT TRIM(name) FROM users;
来源：http://hz.gogol.net.cn/gtaboxvugw.html

[Q85] 数值取整
来源：http://hz.sxryk.cn/gtutvjhclb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yongpay.top/gtyfonrkob.html

[Q86] 读取 JSON 字段
来源：http://hz.zhongyouzk.top/gteycxdklu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.haohaochexian.top/gtuemurjzo.html

[Q87] JSON 字段做条件
来源：http://hz.yvedp.cn/gtmwzxmioz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhongyouzk.top/gtgesojuru.html

[Q88] 行转列（条件聚合）
来源：http://hz.cqqwz.cn/gtkfoiwzbq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hongshengwenyu.top/gtyrdcmcbz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.birdmap.top/gtawicsgjz.html

[Q89] 判断表是否存在
来源：http://hz.xuanzx.com/gtllynxvuu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ehwqpu.com/gtwgvspkos.html

[Q90] 生成序号列
来源：http://hz.xingfuxueyuan.xyz/gtvamgluhs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.9152youxi.cn/gtwljizfhj.html

================================================================================
来源：http://hz.sxryk.cn/gtwuwegbze.html

R. Bash 专题
来源：http://hz.zhengqikj.top/gtjfqqvarj.html

================================================================================
来源：http://hz.yuxming.cn/gtzlxtyhta.html

[R01] shebang 与严格模式
来源：http://hz.iojbl.cn/gtqwgebnft.html

#!/usr/bin/env bash
来源：http://hz.ybcxt.top/gtkrsowrhp.html

set -euo pipefail
来源：http://hz.hysaishi.cn/gtwxxxdzau.html

[R02] 变量赋值与使用
来源：http://hz.jiagoushi.top/gtacymfiri.html

name="Tom"; echo "$name"
来源：http://hz.nanxuanxn.top/gthftdzpux.html

[R03] 只读变量
来源：http://hz.meibo888.top/gtghgonrba.html

readonly PI=3.14
来源：http://hz.jianghu66.top/gttlbvarwm.html

[R04] 位置参数
来源：http://hz.jqgufenzy.top/gtwrldffax.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhengqikj.top/gtvekifosi.html

[R05] 参数默认值
来源：http://hz.yonumen.top/gtxmrzefjs.html

name="${1:-default}"
来源：http://hz.ydzc1.top/gttrceawgc.html

[R06] 判断命令是否存在
来源：http://hz.zdqjudy.top/gtjwsuiabd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.andypj.xyz/gtcuivrqrs.html

[R07] if 判断文件
来源：http://hz.shanyushiyangtech.top/gtvqflgwpc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.c1oappe.top/gtaelpypks.html

[R08] 数值比较
来源：http://hz.zhixingplan.top/gtrnxgntyl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhengqikj.top/gtegkxywgf.html

[R09] 字符串比较
来源：http://hz.jyoumei.cn/gtsgcvpfdr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yanxiufei.cn/gtnhwqzsyz.html

[R10] 正则匹配
来源：http://hz.shanyushiyangtech.top/gtodtoapnj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.snrcjt.cn/gtvwokvpxt.html

[R11] case 多分支
来源：http://hz.hywenlv.cn/gtdxekqrml.html

case "$1" in
来源：http://hz.shzxlz.cn/gtchzhaujj.html

start) echo "启动" ;;
来源：http://hz.yueranfly.top/gtaawbzmfw.html

stop)  echo "停止" ;;
来源：http://hz.c1oappe.top/gtynrozwqi.html

*)     echo "未知命令" ;;
来源：http://hz.hnqzz.top/gtkaypemsn.html

esac
来源：http://hz.ybcxt.top/gtxwqcfgke.html

[R12] for 遍历文件
来源：http://hz.guowangkeji.top/gtuiymszdk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhixingplan.top/gtwdurjtbl.html

[R13] for 计数循环
来源：http://hz.zdqjudy.top/gtqmgnksos.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hnqzz.top/gtkaetdoql.html

[R14] C 风格 for
来源：http://hz.hysaishi.cn/gtqzmssynh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daria6918.cn/gtwcooxdai.html

[R15] while 逐行读文件
来源：http://hz.jyoumei.cn/gthmflunze.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.9152youxi.cn/gtxdnyxtps.html

[R16] until 等待条件
来源：http://hz.ehwqpu.com/gtpbnevaqe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenlongwang.top/gteavpehok.html

[R17] 数组定义与取值
来源：http://hz.shuidangran.top/gtpkidwhnl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhoulong.xyz/gtfbwttbyb.html

[R18] 遍历数组
来源：http://hz.shanyushiyangkeji.top/gtmwdhbjts.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gotoacloud.top/gtvduuyrws.html

[R19] 数组长度
来源：http://hz.hfpthk.cn/gtvdagezqb.html

echo "${#arr[@]}"
来源：http://hz.chenjidiqi.icu/gtbnjpzfpi.html

[R20] 关联数组（字典）
来源：http://hz.xziqi.cn/gttuqyyuhe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258888.top/gtygberqzz.html

[R21] 字符串长度
来源：http://hz.zhiwuduotai.top/gtbflfoiaz.html

echo "${#s}"
来源：http://hz.jinqigufen.top/gtvppnnmun.html

[R22] 截取子串
来源：http://hz.gogol.net.cn/gtfxwbgygp.html

echo "${s:0:5}"
来源：http://hz.nwbrower.top/gtqvawdock.html

[R23] 字符串替换
来源：http://hz.vqdsnc.cn/gtcnnfbhdb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xingfuxueyuan.xyz/gtaaszdvto.html

[R24] 大小写转换
来源：http://hz.ydzc1.top/gtfgvjfqbs.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hnqzz.top/gtfwgggyry.html

[R25] 去后缀 / 去前缀
来源：http://hz.hysaishi.cn/gtgjuvarob.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenjidiqi.icu/gtedohwcgd.html

[R26] 命令替换
来源：http://hz.iojbl.cn/gtqiuzopsv.html

now=$(date +%F); echo "$now"
来源：http://hz.tianlin.xyz/gtnvkfppos.html

[R27] 算术展开
来源：http://hz.jiagoushi.top/gtppbgqbot.html

echo $((1 + 2 * 3))
来源：http://hz.c1oappe.top/gtqsmfuuzb.html

[R28] 浮点运算
来源：http://hz.kuanghao11.cn/gtqalcnbpo.html

echo "scale=2; 10/3" | bc
来源：http://hz.haohaochexian.top/gtfajxzuxh.html

[R29] 定义函数
来源：http://hz.zhiwuduotai.top/gtdvawtlrj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yuanzhike.top/gtsvrxdbcx.html

[R30] 函数返回状态码
来源：http://hz.gaohongyu789.top/gtbydolomj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sxryk.cn/gtlyvyevrj.html

[R31] 局部变量
来源：http://hz.yvedp.cn/gtocfuhndy.html

f() { local x=1; echo "$x"; }
来源：http://hz.havefunace.top/gtbwxovfdl.html

[R32] 参数个数校验
来源：http://hz.chenzaomai.com/gtydfgeomg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gaohongyu789.top/gtyaxfcbon.html

[R33] 捕获错误并提示行号
来源：http://hz.ppjwa.cn/gttzrjzbxc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.quarkkingdee.top/gtlvlnddef.html

[R34] 退出时清理
来源：http://hz.yanxiufei.cn/gtlrrnlkfh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gteuboktyg.html

[R35] 后台执行并等待
来源：http://hz.gotoacloud.top/gtxpzyiwyc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xuanzx.com/gtgyqwxfdb.html

[R36] 并发执行多个任务
来源：http://hz.sxryk.cn/gtmscdwhca.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.dianchejie.cn/gtevalnjfd.html

[R37] 把输出赋给变量
来源：http://hz.aizwys.cn/gtilmizafj.html

files=$(ls -1)
来源：http://hz.hongshengwenyu.top/gtrayxrnje.html

[R38] 管道串联
来源：http://hz.yuxming.cn/gtqfxrjmnk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xuetiantiany.cn/gtmykgihen.html

[R39] 重定向标准输出与错误
来源：http://hz.jianghu66.top/gtqjwkiwef.html

cmd > out.log 2>&1
来源：http://hz.dianchejie.cn/gtqsufcuhk.html

[R40] 追加写日志
来源：http://hz.hammf.cn/gtgeeazkmh.html

echo "log" >> out.log
来源：http://hz.fzhhl.top/gtkjsaefpv.html

[R41] 丢弃输出
来源：http://hz.xingfuxueyuan.xyz/gtllmpvxar.html

cmd >/dev/null 2>&1
来源：http://hz.sufxvd.cn/gtmrqymzzk.html

[R42] 输入重定向
来源：http://hz.jianghu66.top/gtvhyyitge.html

wc -l < a.txt
来源：http://hz.hnxiangtu.top/gtyglaxzmc.html

[R43] 按名字查找文件
来源：http://hz.pengpengdd.cyou/gtzeiexbot.html

find . -name "*.log" -type f
来源：http://hz.birdmap.top/gtfzynodpt.html

[R44] 按修改时间查找
来源：http://hz.yuanzhike.top/gtzzpsmncd.html

find . -mtime -7 -type f
来源：http://hz.zhongyouzk.top/gtrtavbwki.html

[R45] 批量删除
来源：http://hz.svipenyu.cn/gtmsvafjtw.html

find . -name "*.tmp" -delete
来源：http://hz.dianchejie.cn/gtuhlhbpzh.html

[R46] 递归替换文件内容
来源：http://hz.yueranfly.top/gttxxkebgq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.pycfn.com/gtwucloecs.html

[R47] sed 单行替换
来源：http://hz.hnqzz.top/gttkmygbun.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daria6918.cn/gtfkmbczzz.html

[R48] awk 取指定列
来源：http://hz.wangshuangyany.cn/gtbifaitfm.html

awk '{print $1, $3}' a.txt
来源：http://hz.xinyue.icu/gtmxowiglg.html

[R49] awk 带条件
来源：http://hz.yj202588.top/gttevqeetz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shzxlz.cn/gtorntopzy.html

[R50] awk 求和
来源：http://hz.sweek.top/gtwinnjdct.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.quarkkingdee.top/gtlcaruhao.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gtpwwyswpo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydjk.org.cn/gtekrjwtqp.html

[R52] 统计行数
来源：http://hz.aizwys.cn/gtawojmipk.html

wc -l a.txt
来源：http://hz.cdnleiting.top/gtbiqypqaq.html

[R53] 查看文件头与实时尾
来源：http://hz.andypj.xyz/gtaqubvxey.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hfpthk.cn/gtgidbosnj.html

[R54] 比较两个文件
来源：http://hz.snrcjt.cn/gtiunmkrqg.html

diff a.txt b.txt
来源：http://hz.aizwys.cn/gtdiclqaiz.html

[R55] 压缩与解压
来源：http://hz.hnxiangtu.top/gtzsjacush.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gogol.net.cn/gtobqvyqpg.html

[R56] 远程拷贝
来源：http://hz.tianlin.xyz/gtzrmubgri.html

scp file user@host:/path/
来源：http://hz.pengpengdd.cyou/gttluwtkbp.html

[R57] 远程执行命令
来源：http://hz.yj20258888.top/gtxipfwkvs.html

ssh user@host 'uptime'
来源：http://hz.sweek.top/gtqtgvgmeq.html

[R58] 下载文件
来源：http://hz.sweek.top/gtrgqqgdrl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daria6918.cn/gtmolobkwa.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangtech.top/gtjbhiquqh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ybcxt.top/gtoaeeodon.html

[R60] 只看 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gtapzmfgps.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.havefunace.top/gturrpazuc.html

[R61] 磁盘占用
来源：http://hz.shangyingyoupin.top/gttpjkciop.html

df -h;  du -sh *
来源：http://hz.yj202588.top/gtskavxrrx.html

[R62] 找最占空间的文件
来源：http://hz.yonumen.top/gtbuokbzzp.html

du -ah . | sort -rh | head -10
来源：http://hz.xuetiantiany.cn/gtznyikcjp.html

[R63] 内存与进程
来源：http://hz.c1oappe.top/gtmiabkqws.html

free -h;  ps aux | grep nginx
来源：http://hz.pycfn.com/gtxqmuhmrx.html

[R64] 结束进程
来源：http://hz.dianchejie.cn/gtzxgrgefi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.andypj.xyz/gttyszcwjg.html

[R65] 查看端口占用
来源：http://hz.fzhhl.top/gtebbtvyeu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xinyue.icu/gtjhwgxdwt.html

[R66] 定时任务
来源：http://hz.feifeiyinyue.top/gteghoktdg.html

crontab -e;  crontab -l
来源：http://hz.kuanghao11.cn/gteskxilbh.html

[R67] 生成随机十六进制串
来源：http://hz.ydzc1.top/gtczkrkiab.html

openssl rand -hex 16
来源：http://hz.mhx1999.top/gtxntxpeul.html

[R68] 计算文件校验值
来源：http://hz.yongpay.top/gtrpwvoxre.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pengpengdd.cyou/gtmbosgyyi.html

[R69] 生成随机密码
来源：http://hz.jiagoushi.top/gtwncuajog.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhongyouzk.top/gtxgvpbvhk.html

[R70] 时间戳与互转
来源：http://hz.zdqjudy.top/gtdspxblsh.html

date +%s;  date -d @1700000000
来源：http://hz.zhaomingkeji.xyz/gtaamujhon.html

[R71] 日期格式化
来源：http://hz.ydjk.org.cn/gtonnbfxgn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.smart0.xyz/gteuaslsaq.html

[R72] 等待端口就绪
来源：http://hz.shangyingyoupin.top/gtrjaabcdt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.pengpengdd.cyou/gtxlwugcng.html

[R73] 分割大日志
来源：http://hz.shanyushiyangtech.top/gtwaiuzzja.html

split -l 1000 big.log part_
来源：http://hz.xuanzx.com/gtkjahcuaa.html

[R74] 批量重命名
来源：http://hz.jlsjyb.cn/gthsdldecz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.kuanghao11.cn/gtzwzupote.html

[R75] 导出环境变量
来源：http://hz.kuanghao11.cn/gtljtwpzdd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hammf.cn/gtfmkptsnd.html

[R76] 使用临时文件
来源：http://hz.sxryk.cn/gtjqdllofd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daxiang520.top/gtzrrxnssj.html

[R77] 读取用户输入
来源：http://hz.jinqigufen.top/gtfipzwdcu.html

read -rp "请输入: " ans
来源：http://hz.haohaochexian.top/gtyglzmlvx.html

[R78] 交互式菜单
来源：http://hz.hongshengwenyu.top/gtutbjjcdp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.birdmap.top/gttetduedw.html

[R79] 解析命令行选项
来源：http://hz.yj202588.top/gtekurfvyo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daxiang520.top/gtjrxczjao.html

[R80] 查看脚本执行耗时
来源：http://hz.andypj.xyz/gtbqoowfbb.html

time ./run.sh
来源：http://hz.snrcjt.cn/gtmlchzwzc.html

================================================================================
来源：http://hz.zhixingplan.top/gtinxsshfx.html

S. C / C++ 专题
来源：http://hz.yangfankeji.com/gtdxlmibfm.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gthwusiqfb.html

[S01] C：Hello World
来源：http://hz.hongshengwenyu.top/gtxwibzdtn.html

#include <stdio.h>
来源：http://hz.cdnleiting.top/gthxabtvsn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.dianchejie.cn/gtenqlvolm.html

[S02] C：变量与格式化输出
来源：http://hz.birdmap.top/gtuojnmmaz.html

int a = 10; printf("%d\n", a);
来源：http://hz.nwbrower.top/gtpemdznqt.html

[S03] C：读入整数
来源：http://hz.ywan-chungtsiang.top/gtgvxqjzpt.html

int x; scanf("%d", &x);
来源：http://hz.nwbrower.top/gthgvfnnnz.html

[S04] C：字符串复制
来源：http://hz.tianlin.xyz/gtfatsibeb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tian-w.cn/gtrwcthjar.html

[S05] C：字符串长度
来源：http://hz.yvedp.cn/gtzcpqvaer.html

strlen(s)
来源：http://hz.zycfv.cn/gtcpjimpji.html

[S06] C：字符串比较
来源：http://hz.redwolf501.top/gtmylsuvdi.html

strcmp(a, b) == 0
来源：http://hz.zhoulong.xyz/gtxdxjjcop.html

[S07] C：数组遍历求和
来源：http://hz.vqdsnc.cn/gtcohlmggw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yvedp.cn/gtizkssynf.html

[S08] C：动态内存分配与释放
来源：http://hz.zhongyouzk.top/gtrhgiaebf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gogol.net.cn/gtzohzezjy.html

[S09] C：结构体定义与初始化
来源：http://hz.hywenlv.cn/gtmxsggwdz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.wangdashe.top/gtvnhlvdnm.html

[S10] C：指针与解引用
来源：http://hz.sufxvd.cn/gtzehbhvkd.html

int *p = &a;  *p = 5;
来源：http://hz.guowangkeji.top/gttfxqgguf.html

[S11] C：逐行读文件
来源：http://hz.dianchejie.cn/gtichyscmu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj20258.top/gtnwryvqfg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhiwuduotai.top/gteirwjxmh.html

fclose(f);
来源：http://hz.svipenyu.cn/gtjbfwkawx.html

[S12] C：写文件
来源：http://hz.zhixingplan.top/gtivoxmjvl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sysykeji.top/gtznkdfknk.html

[S13] C：宏定义
来源：http://hz.xinyue.icu/gtvdrdiwqe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jianghu66.top/gtlayuklff.html

[S14] C：枚举
来源：http://hz.sufxvd.cn/gtjwniigxr.html


<!-- 参考信息 -->