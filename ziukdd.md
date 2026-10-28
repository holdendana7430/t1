代发 wailian999

[Q44] IN 子查询
来源：http://hz.cashguo.top/gtxqpsmdpz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cheryme.top/gtexhlcspf.html

[Q45] EXISTS 判断存在
来源：http://hz.cucudq.cn/gtqocgytkl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jiagoushi.top/gtvcwugiqi.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shanyushiyangkeji.top/gtwckhtppx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgufenzy.top/gtcsmfzvvg.html

[Q47] 与平均值比较
来源：http://hz.daria6918.cn/gthgcgvjpx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jqgufenzy.top/gtwadlezig.html

[Q48] CTE 公用表表达式
来源：http://hz.yvedp.cn/gtxfthvabk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenjidiqi.icu/gtrmqvxoiu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.meibo888.top/gtdknegxuh.html

[Q49] 更新单行
来源：http://hz.yonumen.top/gtbqqscvpo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nwbrower.top/gtzgekjzrs.html

[Q50] 批量更新
来源：http://hz.gogol.net.cn/gtzpddzauk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cdnleiting.top/gttzpugcmu.html

[Q51] 用子查询更新
来源：http://hz.guowangkeji.top/gtxsttqezo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.aibaodan.cn/gtqpgruuqs.html

[Q52] 删除指定行
来源：http://hz.hammf.cn/gtrvoavoqd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuetiantiany.cn/gttdtftjhb.html

[Q53] 按条件删除
来源：http://hz.xylfe.cn/gtaonnmmfd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnqzz.top/gtbdjxmxiq.html

[Q54] 清空表
来源：http://hz.dashuyun.cn/gtvqswkjlh.html

TRUNCATE TABLE logs;
来源：http://hz.aizwys.cn/gtkubkaubw.html

[Q55] 排名（并列占位）
来源：http://hz.zdqjudy.top/gthuigxfup.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cdnleiting.top/gtiwxkqtyn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gzhubu.top/gtuhhhzwsb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhiwuduotai.top/gtnaqnrvkq.html

[Q57] 行号
来源：http://hz.hnqzz.top/gtxhskjnyd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.quarkkingdee.top/gtvktgmaam.html

[Q58] 累计求和
来源：http://hz.ydjk.org.cn/gthtijpjot.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yuanzhike.top/gtcckgaknd.html

[Q59] 分组内累计
来源：http://hz.havefunace.top/gtmzzdiaxt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.dianchejie.cn/gtmvjpqgkp.html

[Q60] 取上一行 / 下一行
来源：http://hz.shanyushiyangkeji.top/gtnkadvxem.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ywan-chungtsiang.top/gtvcwjriwb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.daria6918.cn/gtckxshyux.html

[Q61] 移动平均
来源：http://hz.ydjk.org.cn/gtimmwctnq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.svipenyu.cn/gtdpmuajhs.html

[Q62] 分组占比
来源：http://hz.smart0.xyz/gtcshmuioc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtvnfehdde.html

[Q63] 开启事务
来源：http://hz.nanxuanxn.top/gtrserseqt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinghuilouyu.cn/gtliahaghu.html

[Q64] 提交事务
来源：http://hz.hammf.cn/gtrqkndojs.html

COMMIT;
来源：http://hz.nanxinkj.top/gtmvzgzbfe.html

[Q65] 回滚事务
来源：http://hz.cheryme.top/gtckyzherq.html

ROLLBACK;
来源：http://hz.gaohongyu789.top/gtjbzsmeun.html

[Q66] 行锁查询
来源：http://hz.shangyingyoupin.top/gtupbzkdwv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.vqdsnc.cn/gtbcpdbrmb.html

[Q67] 设置隔离级别
来源：http://hz.aizwys.cn/gtbmtlgvqg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.meibo888.top/gttaoievcm.html

[Q68] 保存点
来源：http://hz.shangyingyoupin.top/gtgazrjkor.html

SAVEPOINT sp1;
来源：http://hz.bjfxy.top/gtjcxytzkc.html

ROLLBACK TO sp1;
来源：http://hz.hfpthk.cn/gtvecxlaob.html

[Q69] 查看执行计划
来源：http://hz.xuanzx.com/gtjmyrykky.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ydzc1.top/gtpxfvtyhj.html

[Q70] 更新统计信息
来源：http://hz.jiagoushi.top/gtvoyfigfk.html

ANALYZE TABLE users;
来源：http://hz.hongshengwenyu.top/gtoacwuues.html

[Q71] 查看建表语句
来源：http://hz.xingfuxueyuan.xyz/gtzqrqhgyw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinyuanbaomall.cn/gtzmwlcpub.html

[Q72] 查看索引
来源：http://hz.jqgfzy.top/gtpqdknqih.html

SHOW INDEX FROM users;
来源：http://hz.sxryk.cn/gtayxsefdg.html

[Q73] 查看表状态
来源：http://hz.sysykeji.top/gtkqvpgjkm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cheryme.top/gtogmbqulb.html

[Q74] 强制使用索引
来源：http://hz.0kj1m.cn/gtvupjeajr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gogol.net.cn/gtxxdmprbp.html

[Q75] 日期格式化
来源：http://hz.gogol.net.cn/gtuvfezzyu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jyoumei.cn/gtmcdgbzqg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cheryme.top/gtdvajvvdk.html

[Q76] 按天统计
来源：http://hz.xinyue.icu/gtyvynahyg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nwbrower.top/gtdstlibkc.html

[Q77] 时间加减
来源：http://hz.cdnleiting.top/gtsmlyyekx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.svipenyu.cn/gttdccqlyi.html

[Q78] 当前时间
来源：http://hz.jinqigufen.top/gtfdnvrrnd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhongyouzk.top/gtbbnobaye.html

[Q79] 字符串拼接
来源：http://hz.jyoumei.cn/gtfgyugvoo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.316326.xyz/gtmriwkxbe.html

[Q80] 字符串截取
来源：http://hz.jinqigufen.top/gtzzskhakw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xuetiantiany.cn/gtrlrcnrax.html

[Q81] 字符串替换
来源：http://hz.dashuyun.cn/gtodhznbvp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hfpthk.cn/gtsghfstir.html

[Q82] 字符长度与字节长度
来源：http://hz.tanke756.top/gtqzufwnne.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtvbcpqffg.html

[Q83] 大小写转换
来源：http://hz.yangfankeji.com/gtljriagwx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhijiandao.cn/gtftjobbxz.html

[Q84] 去除首尾空格
来源：http://hz.yj20258888.top/gtnpakglgm.html

SELECT TRIM(name) FROM users;
来源：http://hz.sweek.top/gtfmlujret.html

[Q85] 数值取整
来源：http://hz.zhixingplan.top/gtbkivbmke.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hnqzz.top/gtqumzmkcq.html

[Q86] 读取 JSON 字段
来源：http://hz.haohaochexian.top/gtlecbhfjo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.aibaodan.cn/gtfvbzymbh.html

[Q87] JSON 字段做条件
来源：http://hz.yuxming.cn/gtrfyjzswm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuanzx.com/gtwljekayv.html

[Q88] 行转列（条件聚合）
来源：http://hz.ydjk.org.cn/gtednejwub.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xinyue.icu/gtsbiqqqil.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nanxuanxn.top/gtfpmveguk.html

[Q89] 判断表是否存在
来源：http://hz.shuidangran.top/gthwqtceuj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ehwqpu.com/gtlusmfbsq.html

[Q90] 生成序号列
来源：http://hz.ppjwa.cn/gtrnmwslqy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hysaishi.cn/gtnfwkuvzr.html

================================================================================
来源：http://hz.yonumen.top/gtsfwzvjoy.html

R. Bash 专题
来源：http://hz.kuanghao11.cn/gtuhiqogxm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtvqujiton.html

[R01] shebang 与严格模式
来源：http://hz.jinyuanbaomall.cn/gtoxrkcrtu.html

#!/usr/bin/env bash
来源：http://hz.xuanzx.com/gtooezcylg.html

set -euo pipefail
来源：http://hz.xylfe.cn/gtvntibkhy.html

[R02] 变量赋值与使用
来源：http://hz.vqdsnc.cn/gtddydpakq.html

name="Tom"; echo "$name"
来源：http://hz.hnxiangtu.top/gtflrkciab.html

[R03] 只读变量
来源：http://hz.tianlin.xyz/gtgtzijdnv.html

readonly PI=3.14
来源：http://hz.jqgfzy.top/gtbkrfsanf.html

[R04] 位置参数
来源：http://hz.shanyushiyangtech.top/gtnbnxbcsq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.9152youxi.cn/gtziussogf.html

[R05] 参数默认值
来源：http://hz.daria6918.cn/gtbhamqfho.html

name="${1:-default}"
来源：http://hz.tian-w.cn/gtiucyppwz.html

[R06] 判断命令是否存在
来源：http://hz.gotoacloud.top/gtmkyifjhq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtzcocmvti.html

[R07] if 判断文件
来源：http://hz.jinqigfzy.top/gtnrnazwro.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jyoumei.cn/gtcuhhchjw.html

[R08] 数值比较
来源：http://hz.c1oappe.top/gtgpgegtzr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangdashe.top/gtbuawrosz.html

[R09] 字符串比较
来源：http://hz.tanke756.top/gtggkwddbw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhixingplan.top/gtnvyfvoaj.html

[R10] 正则匹配
来源：http://hz.zdqjudy.top/gtvjjuxqlr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cashguo.top/gtuxkwgvwx.html

[R11] case 多分支
来源：http://hz.cucudq.cn/gtczssatqo.html

case "$1" in
来源：http://hz.hywenlv.cn/gtyyakavwi.html

start) echo "启动" ;;
来源：http://hz.birdmap.top/gtfgjombxw.html

stop)  echo "停止" ;;
来源：http://hz.daria6918.cn/gtpsppikit.html

*)     echo "未知命令" ;;
来源：http://hz.zhijiandao.cn/gtgkkucfpf.html

esac
来源：http://hz.gogol.net.cn/gtzyigykmt.html

[R12] for 遍历文件
来源：http://hz.yuanzhike.top/gtoeyhjvyb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.dianchejie.cn/gtpktwgxgt.html

[R13] for 计数循环
来源：http://hz.gogol.net.cn/gtccaghvjl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jyoumei.cn/gtoiuwuykt.html

[R14] C 风格 for
来源：http://hz.kuanghao11.cn/gtxvuwimfo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.birdmap.top/gtwrehmhfp.html

[R15] while 逐行读文件
来源：http://hz.zhoulong.xyz/gtylieppcy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sysykeji.top/gtkkbfoltr.html

[R16] until 等待条件
来源：http://hz.pycfn.com/gtpzljkpqb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ywan-chungtsiang.top/gthqvldsme.html

[R17] 数组定义与取值
来源：http://hz.svipenyu.cn/gtbdbeyrlm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.feifeiyinyue.top/gtyvmksiry.html

[R18] 遍历数组
来源：http://hz.pengpengdd.cyou/gthqczeosc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yongpay.top/gtyixrkuvy.html

[R19] 数组长度
来源：http://hz.tanke756.top/gtzqhbzetv.html

echo "${#arr[@]}"
来源：http://hz.dashuyun.cn/gtslgkdtwt.html

[R20] 关联数组（字典）
来源：http://hz.chenjidiqi.icu/gtpmpajtvd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yangfankeji.com/gtccddjqjn.html

[R21] 字符串长度
来源：http://hz.sysykeji.top/gtqwjxxmrc.html

echo "${#s}"
来源：http://hz.bjfxy.top/gtwwyeuriy.html

[R22] 截取子串
来源：http://hz.yanxiufei.cn/gtlheclspt.html

echo "${s:0:5}"
来源：http://hz.xziqi.cn/gtgwkczfop.html

[R23] 字符串替换
来源：http://hz.ppjwa.cn/gtffuhfdky.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.birdmap.top/gttanbceqb.html

[R24] 大小写转换
来源：http://hz.316326.xyz/gtcupvfzcy.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenzaomai.com/gtnppcapqn.html

[R25] 去后缀 / 去前缀
来源：http://hz.bjfxy.top/gtkcdjmrxg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yongpay.top/gtnlopvgrm.html

[R26] 命令替换
来源：http://hz.havefunace.top/gtyophyffj.html

now=$(date +%F); echo "$now"
来源：http://hz.andypj.xyz/gtwhhoxswa.html

[R27] 算术展开
来源：http://hz.pengpengdd.cyou/gtgvlahvhr.html

echo $((1 + 2 * 3))
来源：http://hz.yongpay.top/gtsnxgxozz.html

[R28] 浮点运算
来源：http://hz.ydzc1.top/gtdxrovwww.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhijiandao.cn/gtlvhhmmsn.html

[R29] 定义函数
来源：http://hz.zhengqikj.top/gtpbinuibj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hammf.cn/gtivouwegb.html

[R30] 函数返回状态码
来源：http://hz.aizwys.cn/gttwghkxiw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.haohaochexian.top/gtilxecdiy.html

[R31] 局部变量
来源：http://hz.hfpthk.cn/gtsdgqfssb.html

f() { local x=1; echo "$x"; }
来源：http://hz.quarkkingdee.top/gthuyukmdf.html

[R32] 参数个数校验
来源：http://hz.9152youxi.cn/gtzbgezapg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.snrcjt.cn/gtuqrrkiej.html

[R33] 捕获错误并提示行号
来源：http://hz.jqgufenzy.top/gtuzqhfvpn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ydzc1.top/gtbulqpyxw.html

[R34] 退出时清理
来源：http://hz.sysykeji.top/gtcfjdedtp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtkaazwwqp.html

[R35] 后台执行并等待
来源：http://hz.dashuyun.cn/gtdadushqv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.meibo888.top/gtrhsgfqri.html

[R36] 并发执行多个任务
来源：http://hz.zhaomingkeji.xyz/gtewmhwllh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.pengpengdd.cyou/gtiweizift.html

[R37] 把输出赋给变量
来源：http://hz.pycfn.com/gtmalbxsrp.html

files=$(ls -1)
来源：http://hz.chenjidiqi.icu/gtqunqzygl.html

[R38] 管道串联
来源：http://hz.jyoumei.cn/gtlkcjjljt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.birdmap.top/gtaeptqrlm.html

[R39] 重定向标准输出与错误
来源：http://hz.xylfe.cn/gtvfologot.html

cmd > out.log 2>&1
来源：http://hz.zhijiandao.cn/gtzbgugvic.html

[R40] 追加写日志
来源：http://hz.tianlin.xyz/gtznrwmimh.html

echo "log" >> out.log
来源：http://hz.shanyushiyangkeji.top/gttzlbclga.html

[R41] 丢弃输出
来源：http://hz.hongshengwenyu.top/gtjbpqyfyw.html

cmd >/dev/null 2>&1
来源：http://hz.nanxinkj.top/gtsxwqugrk.html

[R42] 输入重定向
来源：http://hz.shanyushiyangkeji.top/gtzmpsifie.html

wc -l < a.txt
来源：http://hz.gogol.net.cn/gtpjlnilhr.html

[R43] 按名字查找文件
来源：http://hz.jinqigufen.top/gtohkojkbf.html

find . -name "*.log" -type f
来源：http://hz.mhx1999.top/gtfmoyvkgc.html

[R44] 按修改时间查找
来源：http://hz.ywan-chungtsiang.top/gtoikffloz.html

find . -mtime -7 -type f
来源：http://hz.cdnleiting.top/gtocsbthee.html

[R45] 批量删除
来源：http://hz.jlsjyb.cn/gtfhdqyxvl.html

find . -name "*.tmp" -delete
来源：http://hz.hnxiangtu.top/gtcmfglffw.html

[R46] 递归替换文件内容
来源：http://hz.zhaomingkeji.xyz/gtwankgxpr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.tianlin.xyz/gtnjzsffvu.html

[R47] sed 单行替换
来源：http://hz.tian-w.cn/gtwtnpujwj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenjidiqi.icu/gtmxhzpjeg.html

[R48] awk 取指定列
来源：http://hz.hfpthk.cn/gtbcwoegez.html

awk '{print $1, $3}' a.txt
来源：http://hz.meibo888.top/gtfeggdscb.html

[R49] awk 带条件
来源：http://hz.zhongyouzk.top/gtdpheladg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ehwqpu.com/gtwqauwhsr.html

[R50] awk 求和
来源：http://hz.sxryk.cn/gtgzulndkw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sweek.top/gtbjqqqxle.html

[R51] 排序去重取前几
来源：http://hz.ydjk.org.cn/gtcvvcohge.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.guannengcc.top/gtpsanvjvv.html

[R52] 统计行数
来源：http://hz.zhaomingkeji.xyz/gtogbqleli.html

wc -l a.txt
来源：http://hz.xziqi.cn/gtetmplmbb.html

[R53] 查看文件头与实时尾
来源：http://hz.xinyue.icu/gtyevdzqkt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nanxinkj.top/gtigkisjyu.html

[R54] 比较两个文件
来源：http://hz.sxryk.cn/gtlyoojdrq.html

diff a.txt b.txt
来源：http://hz.nanxuanxn.top/gtddsaulcf.html

[R55] 压缩与解压
来源：http://hz.dashuyun.cn/gtkbffuica.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.kuanghao11.cn/gttotoweug.html

[R56] 远程拷贝
来源：http://hz.jianghu66.top/gtvliplzoe.html

scp file user@host:/path/
来源：http://hz.jinqigufen.top/gtqqlijmvw.html

[R57] 远程执行命令
来源：http://hz.sufxvd.cn/gtkbgcvteq.html

ssh user@host 'uptime'
来源：http://hz.jlsjyb.cn/gtsdkmnwle.html

[R58] 下载文件
来源：http://hz.xuanzx.com/gtupjzojjc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xuanzx.com/gtktvzivjo.html

[R59] 发 POST JSON
来源：http://hz.zdqjudy.top/gtvbhvhfcz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pengpengdd.cyou/gtygtbfsgu.html

[R60] 只看 HTTP 状态码
来源：http://hz.gotoacloud.top/gtulxzeice.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.guowangkeji.top/gtdiywbggo.html

[R61] 磁盘占用
来源：http://hz.fengsongda.top/gtrjdliwyg.html

df -h;  du -sh *
来源：http://hz.xylfe.cn/gtuywhhxzf.html

[R62] 找最占空间的文件
来源：http://hz.shangyingyoupin.top/gtbaerbcha.html

du -ah . | sort -rh | head -10
来源：http://hz.c1oappe.top/gtskblmwrj.html

[R63] 内存与进程
来源：http://hz.zhengqikj.top/gtnkmsiitc.html

free -h;  ps aux | grep nginx
来源：http://hz.jlsjyb.cn/gtxobdflsy.html

[R64] 结束进程
来源：http://hz.bjfxy.top/gtuqbslecx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shanyushiyangkeji.top/gtjbfyihmw.html

[R65] 查看端口占用
来源：http://hz.xuanzx.com/gtpmgctylf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.redwolf501.top/gtatgwamip.html

[R66] 定时任务
来源：http://hz.meibo888.top/gtwlexbago.html

crontab -e;  crontab -l
来源：http://hz.fengsongda.top/gtpnrxjynk.html

[R67] 生成随机十六进制串
来源：http://hz.hnxiangtu.top/gtykxjtkzq.html

openssl rand -hex 16
来源：http://hz.sweek.top/gtksiobhgc.html

[R68] 计算文件校验值
来源：http://hz.hnxiangtu.top/gtwqxqvzsq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yj202588.top/gtxuqeydcr.html

[R69] 生成随机密码
来源：http://hz.aizwys.cn/gtvqewwjku.html

head -c 16 /dev/urandom | base64
来源：http://hz.mhx1999.top/gtqfmplsie.html

[R70] 时间戳与互转
来源：http://hz.quarkkingdee.top/gtlqprndpt.html

date +%s;  date -d @1700000000
来源：http://hz.zhixingplan.top/gtybhdyhpq.html

[R71] 日期格式化
来源：http://hz.xuanzx.com/gtgxfdawff.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gaohongyu789.top/gtfnnakrjq.html

[R72] 等待端口就绪
来源：http://hz.chenjidiqi.icu/gthukfxcii.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xingfuxueyuan.xyz/gtrwjcnjrn.html

[R73] 分割大日志
来源：http://hz.c1oappe.top/gtzagbcqob.html

split -l 1000 big.log part_
来源：http://hz.havefunace.top/gtraewcqej.html

[R74] 批量重命名
来源：http://hz.zdqjudy.top/gtfrvwllvq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.aibaodan.cn/gtwrsipoqc.html

[R75] 导出环境变量
来源：http://hz.cucudq.cn/gtjctbdvae.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhiwuduotai.top/gtpbrqhsbl.html

[R76] 使用临时文件
来源：http://hz.wangshuangyany.cn/gtvbsfymqr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.9152youxi.cn/gtmwewdhjj.html

[R77] 读取用户输入
来源：http://hz.chenlongwang.top/gtukhaluvv.html

read -rp "请输入: " ans
来源：http://hz.aizwys.cn/gtaewwpywl.html

[R78] 交互式菜单
来源：http://hz.dianchejie.cn/gthtbgdaml.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yangfankeji.com/gtfzixolyy.html

[R79] 解析命令行选项
来源：http://hz.tian-w.cn/gtgjulmxxn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuxming.cn/gtyhkyxncz.html

[R80] 查看脚本执行耗时
来源：http://hz.zhijiandao.cn/gtpxmonqcb.html

time ./run.sh
来源：http://hz.wangshuangyany.cn/gtggpxobww.html

================================================================================
来源：http://hz.kuanghao11.cn/gtbgraapnn.html

S. C / C++ 专题
来源：http://hz.sweek.top/gtomropgzc.html

================================================================================
来源：http://hz.zhixingplan.top/gtoutivfpx.html

[S01] C：Hello World
来源：http://hz.yonumen.top/gthaliovzt.html

#include <stdio.h>
来源：http://hz.zhengqikj.top/gtjbwmatty.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jqgfzy.top/gtidxtuwls.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangtech.top/gtsrsfhvpf.html

int a = 10; printf("%d\n", a);
来源：http://hz.ydzc1.top/gthzgvazkv.html

[S03] C：读入整数
来源：http://hz.gaohongyu789.top/gtlrhaebic.html

int x; scanf("%d", &x);
来源：http://hz.hammf.cn/gtdmgwellk.html

[S04] C：字符串复制
来源：http://hz.tian-w.cn/gtxmmrzzkt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hysaishi.cn/gtijofpayf.html

[S05] C：字符串长度
来源：http://hz.zhijiandao.cn/gtqjnbqliy.html

strlen(s)
来源：http://hz.jyoumei.cn/gtsgtgyrbs.html

[S06] C：字符串比较
来源：http://hz.tian-w.cn/gtfdojfsag.html

strcmp(a, b) == 0
来源：http://hz.kuanghao11.cn/gtwavrrqqj.html

[S07] C：数组遍历求和
来源：http://hz.mhx1999.top/gtnbouicum.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinqigufen.top/gtkdgqoyhz.html

[S08] C：动态内存分配与释放
来源：http://hz.yangfankeji.com/gtgsebqzqr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnxiangtu.top/gtgoljapbu.html

[S09] C：结构体定义与初始化
来源：http://hz.wangdashe.top/gtbqgrgwvz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zycfv.cn/gtrphmxqcn.html

[S10] C：指针与解引用
来源：http://hz.yangfankeji.com/gttlyensyw.html

int *p = &a;  *p = 5;
来源：http://hz.feifeiyinyue.top/gtggpipptv.html

[S11] C：逐行读文件
来源：http://hz.ehwqpu.com/gthqvvwhac.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.daria6918.cn/gticszemoz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.52xcode.cn/gtkihokqig.html

fclose(f);
来源：http://hz.tianlin.xyz/gthwjkcomo.html

[S12] C：写文件
来源：http://hz.mhx1999.top/gtxvfjxfjh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.meibo888.top/gtomnrevax.html

[S13] C：宏定义
来源：http://hz.zhijiandao.cn/gtbqxqpzji.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.fengsongda.top/gtpmyvpqil.html

[S14] C：枚举
来源：http://hz.birdmap.top/gtvszinvif.html


<!-- 参考信息 -->