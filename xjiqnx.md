代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gogol.net.cn/gtvdouvttd.html

[Q54] 清空表
来源：http://hz.chenjidiqi.icu/gtphiifxoo.html

TRUNCATE TABLE logs;
来源：http://hz.ywan-chungtsiang.top/gtgbgrqclq.html

[Q55] 排名（并列占位）
来源：http://hz.jiagoushi.top/gtpfwlxdvk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinyuanbaomall.cn/gtfjffzfya.html

[Q56] 密集排名（并列不占位）
来源：http://hz.chenlongwang.top/gtgymjfaek.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shanyushiyangtech.top/gtqaxlbdvj.html

[Q57] 行号
来源：http://hz.zhaomingkeji.xyz/gtkiabzrzg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jianghu66.top/gtrsdyelnu.html

[Q58] 累计求和
来源：http://hz.yanxiufei.cn/gtacjpnjyv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shuidangran.top/gthjtoyqjd.html

[Q59] 分组内累计
来源：http://hz.yangfankeji.com/gttzyaamur.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ybcxt.top/gtxqmetcnk.html

[Q60] 取上一行 / 下一行
来源：http://hz.yueranfly.top/gtzpozshpo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenlongwang.top/gtdmykcdip.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xziqi.cn/gtvkjqovjr.html

[Q61] 移动平均
来源：http://hz.wangshuangyany.cn/gtxzqkkked.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.smart0.xyz/gtmktmsnfn.html

[Q62] 分组占比
来源：http://hz.yonumen.top/gtocupfwbw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtlhxumcym.html

[Q63] 开启事务
来源：http://hz.birdmap.top/gtghwimrgu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.wangshuangyany.cn/gtfsurleaf.html

[Q64] 提交事务
来源：http://hz.chenlongwang.top/gtkskxeyfe.html

COMMIT;
来源：http://hz.yj20258888.top/gtbioghcux.html

[Q65] 回滚事务
来源：http://hz.xziqi.cn/gtoigwygfr.html

ROLLBACK;
来源：http://hz.jyoumei.cn/gtgqbkmmmt.html

[Q66] 行锁查询
来源：http://hz.mhx1999.top/gtvmvjfwgj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.havefunace.top/gtwlqyuhbh.html

[Q67] 设置隔离级别
来源：http://hz.iojbl.cn/gtcdogtkqa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhiwuduotai.top/gtasfxdlie.html

[Q68] 保存点
来源：http://hz.tian-w.cn/gtetshdtqt.html

SAVEPOINT sp1;
来源：http://hz.zhixingplan.top/gtnwbhbklv.html

ROLLBACK TO sp1;
来源：http://hz.yj20258.top/gtoeorusxf.html

[Q69] 查看执行计划
来源：http://hz.iojbl.cn/gtalguuulm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tanke756.top/gtzbcthmog.html

[Q70] 更新统计信息
来源：http://hz.nanxinkj.top/gtrlylgdvc.html

ANALYZE TABLE users;
来源：http://hz.ybcxt.top/gtrukgejdh.html

[Q71] 查看建表语句
来源：http://hz.bjfxy.top/gtipukikzt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.smart0.xyz/gtvcoevzbg.html

[Q72] 查看索引
来源：http://hz.hnqzz.top/gtoqtcszyy.html

SHOW INDEX FROM users;
来源：http://hz.andypj.xyz/gtpcoubfyt.html

[Q73] 查看表状态
来源：http://hz.ywan-chungtsiang.top/gtykdtgrpb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gzhubu.top/gtwhstsyck.html

[Q74] 强制使用索引
来源：http://hz.zhaomingkeji.xyz/gtxdyrmlst.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gtuyckudvi.html

[Q75] 日期格式化
来源：http://hz.xylfe.cn/gtyqmdkvgw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtqoauwiod.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ydzc1.top/gtzhshaddq.html

[Q76] 按天统计
来源：http://hz.jqgfzy.top/gtahibfffo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gzhubu.top/gtadxmjjna.html

[Q77] 时间加减
来源：http://hz.jqgfzy.top/gtrukqwskx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jiagoushi.top/gtcgdigipx.html

[Q78] 当前时间
来源：http://hz.yvedp.cn/gtbhnesyas.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fengsongda.top/gthslfibmp.html

[Q79] 字符串拼接
来源：http://hz.xinyue.icu/gtnmhhqgcn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.havefunace.top/gtesduhejr.html

[Q80] 字符串截取
来源：http://hz.sweek.top/gtxtwwxssm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.guannengcc.top/gtfygyqrot.html

[Q81] 字符串替换
来源：http://hz.quarkkingdee.top/gtbzttcyql.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yuxming.cn/gtgyjutpie.html

[Q82] 字符长度与字节长度
来源：http://hz.chenlongwang.top/gtklcidfvv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cqqwz.cn/gtgqugestk.html

[Q83] 大小写转换
来源：http://hz.bjfxy.top/gtibtobcbk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yangfankeji.com/gtkyjrjbmb.html

[Q84] 去除首尾空格
来源：http://hz.chenlongwang.top/gtxczqogad.html

SELECT TRIM(name) FROM users;
来源：http://hz.zycfv.cn/gtbefosilo.html

[Q85] 数值取整
来源：http://hz.0kj1m.cn/gtdyulxvub.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yvedp.cn/gtijhmwapk.html

[Q86] 读取 JSON 字段
来源：http://hz.andypj.xyz/gtoyhyimep.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.redwolf501.top/gtjjijulgh.html

[Q87] JSON 字段做条件
来源：http://hz.9152youxi.cn/gtvmfjcajf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jyoumei.cn/gtvntdjort.html

[Q88] 行转列（条件聚合）
来源：http://hz.mhx1999.top/gtegrfitzt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenlongwang.top/gtcpxktrkq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sweek.top/gtqoufxijg.html

[Q89] 判断表是否存在
来源：http://hz.zhixingplan.top/gthcvmvflu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guowangkeji.top/gtrmwtuizl.html

[Q90] 生成序号列
来源：http://hz.zhixingplan.top/gthdcezllt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.316326.xyz/gtfslkykzd.html

================================================================================
来源：http://hz.yuanzhike.top/gthjklwccl.html

R. Bash 专题
来源：http://hz.iojbl.cn/gtbtursizp.html

================================================================================
来源：http://hz.jqgufenzy.top/gthreubkto.html

[R01] shebang 与严格模式
来源：http://hz.cqqwz.cn/gtrkznzths.html

#!/usr/bin/env bash
来源：http://hz.sufxvd.cn/gtpkwckils.html

set -euo pipefail
来源：http://hz.feifeiyinyue.top/gtcmfbgpgb.html

[R02] 变量赋值与使用
来源：http://hz.xziqi.cn/gtwldrqqjm.html

name="Tom"; echo "$name"
来源：http://hz.yvedp.cn/gthsvrwppv.html

[R03] 只读变量
来源：http://hz.nanxuanxn.top/gtcgiqozel.html

readonly PI=3.14
来源：http://hz.ehwqpu.com/gtrwmyosey.html

[R04] 位置参数
来源：http://hz.yangfankeji.com/gtmytrzmox.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinyuanbaomall.cn/gtevuzepwn.html

[R05] 参数默认值
来源：http://hz.ydzc1.top/gtsygakjhf.html

name="${1:-default}"
来源：http://hz.jinqigufen.top/gttwbpwzxe.html

[R06] 判断命令是否存在
来源：http://hz.yuxming.cn/gtwhhxbxjx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ppjwa.cn/gtlxnsoscz.html

[R07] if 判断文件
来源：http://hz.shzxlz.cn/gtmygzbqnd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sufxvd.cn/gtrgcorpdh.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gtwekjrgco.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ybcxt.top/gthkmqeogs.html

[R09] 字符串比较
来源：http://hz.sysykeji.top/gtreuaxykl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ivvv.top/gtxaymsaou.html

[R10] 正则匹配
来源：http://hz.quarkkingdee.top/gtkvmbsbzi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.wangdashe.top/gtgiguanfh.html

[R11] case 多分支
来源：http://hz.birdmap.top/gtrjtguhcf.html

case "$1" in
来源：http://hz.kuanghao11.cn/gtnswzkyvd.html

start) echo "启动" ;;
来源：http://hz.redwolf501.top/gtsxsdyyrr.html

stop)  echo "停止" ;;
来源：http://hz.zhongyouzk.top/gtzefewlha.html

*)     echo "未知命令" ;;
来源：http://hz.zhixingplan.top/gtbkygrpry.html

esac
来源：http://hz.gaohongyu789.top/gtemghirzi.html

[R12] for 遍历文件
来源：http://hz.hammf.cn/gtdfpwedfp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.feifeiyinyue.top/gtbknlcqqx.html

[R13] for 计数循环
来源：http://hz.jinqigufen.top/gtcoslaqvq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.fengsongda.top/gtaftpevuw.html

[R14] C 风格 for
来源：http://hz.sysykeji.top/gtmkbbhzau.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.kuanghao11.cn/gthhokljhv.html

[R15] while 逐行读文件
来源：http://hz.haohaochexian.top/gtdqveilic.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhixingplan.top/gthltbsjij.html

[R16] until 等待条件
来源：http://hz.gogol.net.cn/gtapfrycmc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tianlin.xyz/gtxmjsdutc.html

[R17] 数组定义与取值
来源：http://hz.yj202588.top/gtuarmflch.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zdqjudy.top/gtwbonsvjo.html

[R18] 遍历数组
来源：http://hz.xuanzx.com/gtowjnccsp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hfpthk.cn/gtyisloeqj.html

[R19] 数组长度
来源：http://hz.mhx1999.top/gtmtltusiz.html

echo "${#arr[@]}"
来源：http://hz.zhongyouzk.top/gtshtldcep.html

[R20] 关联数组（字典）
来源：http://hz.yuanzhike.top/gtollrgypf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhaomingkeji.xyz/gtzocntqus.html

[R21] 字符串长度
来源：http://hz.xuetiantiany.cn/gtvmrfqmdt.html

echo "${#s}"
来源：http://hz.tian-w.cn/gtkkreuvqo.html

[R22] 截取子串
来源：http://hz.gaohongyu789.top/gtzqpttuws.html

echo "${s:0:5}"
来源：http://hz.zhaomingkeji.xyz/gtwslaxrkj.html

[R23] 字符串替换
来源：http://hz.bjfxy.top/gtsjbjidiv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hywenlv.cn/gtbijhmoda.html

[R24] 大小写转换
来源：http://hz.jinghuilouyu.cn/gtvmdxizqq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dashuyun.cn/gtrzeeiual.html

[R25] 去后缀 / 去前缀
来源：http://hz.quarkkingdee.top/gtouvbyohj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tian-w.cn/gtucfoglkj.html

[R26] 命令替换
来源：http://hz.hnqzz.top/gtsavyealh.html

now=$(date +%F); echo "$now"
来源：http://hz.xinyue.icu/gtyvhbnwrb.html

[R27] 算术展开
来源：http://hz.xinyue.icu/gtqacqvxrf.html

echo $((1 + 2 * 3))
来源：http://hz.haohaochexian.top/gtfidqauic.html

[R28] 浮点运算
来源：http://hz.meibo888.top/gtihqimfge.html

echo "scale=2; 10/3" | bc
来源：http://hz.cashguo.top/gtldggimfx.html

[R29] 定义函数
来源：http://hz.xingfuxueyuan.xyz/gtuhfxwdyj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258888.top/gtsrqhkxqf.html

[R30] 函数返回状态码
来源：http://hz.aizwys.cn/gtppbmlkaf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xinyue.icu/gtaouekbri.html

[R31] 局部变量
来源：http://hz.gogol.net.cn/gtdnnxwfym.html

f() { local x=1; echo "$x"; }
来源：http://hz.cashguo.top/gtceuyuiak.html

[R32] 参数个数校验
来源：http://hz.kuanghao11.cn/gtlhoholhk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ivvv.top/gtlffvwace.html

[R33] 捕获错误并提示行号
来源：http://hz.jyoumei.cn/gtzofufhxf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.havefunace.top/gtzhotdqjh.html

[R34] 退出时清理
来源：http://hz.quarkkingdee.top/gtdjjquftn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258888.top/gtucihxyzj.html

[R35] 后台执行并等待
来源：http://hz.hammf.cn/gtdwbxbeio.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinyuanbaomall.cn/gtdnaptxmv.html

[R36] 并发执行多个任务
来源：http://hz.yangfankeji.com/gtoytendnx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhixingplan.top/gtevzfmhmi.html

[R37] 把输出赋给变量
来源：http://hz.hongshengwenyu.top/gtxrziezpe.html

files=$(ls -1)
来源：http://hz.quarkkingdee.top/gtbvdkpazl.html

[R38] 管道串联
来源：http://hz.ybcxt.top/gtfthpgtkb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xylfe.cn/gtavhqgeci.html

[R39] 重定向标准输出与错误
来源：http://hz.daria6918.cn/gtjjlbsblg.html

cmd > out.log 2>&1
来源：http://hz.hongshengwenyu.top/gtshqqxtfb.html

[R40] 追加写日志
来源：http://hz.sxryk.cn/gtoviacpwr.html

echo "log" >> out.log
来源：http://hz.ehwqpu.com/gtsvohqqgr.html

[R41] 丢弃输出
来源：http://hz.shuidangran.top/gtztscwwkp.html

cmd >/dev/null 2>&1
来源：http://hz.andypj.xyz/gtvsmyzgdt.html

[R42] 输入重定向
来源：http://hz.zhongyouzk.top/gtrehrnuwx.html

wc -l < a.txt
来源：http://hz.sufxvd.cn/gtnfrckgmk.html

[R43] 按名字查找文件
来源：http://hz.ybcxt.top/gtogqpexji.html

find . -name "*.log" -type f
来源：http://hz.havefunace.top/gtywbmjnjd.html

[R44] 按修改时间查找
来源：http://hz.nwbrower.top/gtryxcwyph.html

find . -mtime -7 -type f
来源：http://hz.dashuyun.cn/gtzptxmmoy.html

[R45] 批量删除
来源：http://hz.fzhhl.top/gtncezhlha.html

find . -name "*.tmp" -delete
来源：http://hz.jinqigfzy.top/gtkliwlhwo.html

[R46] 递归替换文件内容
来源：http://hz.yonumen.top/gtnhhpdgrf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhoulong.xyz/gtejjqdokg.html

[R47] sed 单行替换
来源：http://hz.gaohongyu789.top/gtcsbxdkwt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dashuyun.cn/gtbulyblkl.html

[R48] awk 取指定列
来源：http://hz.shangyingyoupin.top/gtbbizslvd.html

awk '{print $1, $3}' a.txt
来源：http://hz.xylfe.cn/gtdgtlslnj.html

[R49] awk 带条件
来源：http://hz.yueranfly.top/gtwbgmkamf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.guannengcc.top/gtypjtnghe.html

[R50] awk 求和
来源：http://hz.jinghuilouyu.cn/gtbdyncaxx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj202588.top/gtqljbfsqa.html

[R51] 排序去重取前几
来源：http://hz.fengsongda.top/gtpxibfyur.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.haohaochexian.top/gtfpunszsb.html

[R52] 统计行数
来源：http://hz.jyoumei.cn/gtszlqgups.html

wc -l a.txt
来源：http://hz.c1oappe.top/gtrwtweqbg.html

[R53] 查看文件头与实时尾
来源：http://hz.xziqi.cn/gtxsfiisem.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinqigfzy.top/gtatumbaqn.html

[R54] 比较两个文件
来源：http://hz.zhijiandao.cn/gtzzysnyax.html

diff a.txt b.txt
来源：http://hz.9152youxi.cn/gtvqwbslvn.html

[R55] 压缩与解压
来源：http://hz.gaohongyu789.top/gtfvmwazow.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cucudq.cn/gtbsjipcfn.html

[R56] 远程拷贝
来源：http://hz.yongpay.top/gtwqhxabwv.html

scp file user@host:/path/
来源：http://hz.smart0.xyz/gtxvosrlgk.html

[R57] 远程执行命令
来源：http://hz.chenlongwang.top/gtspvrsbrr.html

ssh user@host 'uptime'
来源：http://hz.cdnleiting.top/gtohkjjdzb.html

[R58] 下载文件
来源：http://hz.wangshuangyany.cn/gtxuutqtjk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.meibo888.top/gtbuncesag.html

[R59] 发 POST JSON
来源：http://hz.zhixingplan.top/gtusjfdnyf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.snrcjt.cn/gtrjeapqyw.html

[R60] 只看 HTTP 状态码
来源：http://hz.cdnleiting.top/gtftbcqqmk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.redwolf501.top/gtdkldayon.html

[R61] 磁盘占用
来源：http://hz.cucudq.cn/gthgrnknvs.html

df -h;  du -sh *
来源：http://hz.nwbrower.top/gtprsxdorn.html

[R62] 找最占空间的文件
来源：http://hz.hfpthk.cn/gtxvoreqoq.html

du -ah . | sort -rh | head -10
来源：http://hz.zdqjudy.top/gtiqguwcxz.html

[R63] 内存与进程
来源：http://hz.shzxlz.cn/gtbydkkqvz.html

free -h;  ps aux | grep nginx
来源：http://hz.pycfn.com/gtnozqoxji.html

[R64] 结束进程
来源：http://hz.sysykeji.top/gtofzswjvz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigfzy.top/gtpbkodewp.html

[R65] 查看端口占用
来源：http://hz.dashuyun.cn/gtwoowhrkk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgfzy.top/gtymfskimy.html

[R66] 定时任务
来源：http://hz.svipenyu.cn/gtkgosscpg.html

crontab -e;  crontab -l
来源：http://hz.daria6918.cn/gtuebinxhg.html

[R67] 生成随机十六进制串
来源：http://hz.zdqjudy.top/gtastjyuxu.html

openssl rand -hex 16
来源：http://hz.chenjidiqi.icu/gtjyqyoxmx.html

[R68] 计算文件校验值
来源：http://hz.zhengqikj.top/gtgxlnpmvb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgfzy.top/gtmlojbygl.html

[R69] 生成随机密码
来源：http://hz.hnxiangtu.top/gtpzfyybsr.html

head -c 16 /dev/urandom | base64
来源：http://hz.shangyingyoupin.top/gtzhdtncqi.html

[R70] 时间戳与互转
来源：http://hz.hfpthk.cn/gtnqeeilbf.html

date +%s;  date -d @1700000000
来源：http://hz.kuanghao11.cn/gtyykfyzka.html

[R71] 日期格式化
来源：http://hz.yuanzhike.top/gtyqjqxgvv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuanzx.com/gtkypmfsbd.html

[R72] 等待端口就绪
来源：http://hz.jiagoushi.top/gtbcjlvsbv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.tianlin.xyz/gtciftbgkv.html

[R73] 分割大日志
来源：http://hz.sysykeji.top/gthwytafzn.html

split -l 1000 big.log part_
来源：http://hz.mhx1999.top/gtzopwqpmh.html

[R74] 批量重命名
来源：http://hz.zhengqikj.top/gtettmlhgi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xinyue.icu/gtllegiint.html

[R75] 导出环境变量
来源：http://hz.zdqjudy.top/gtwovaiiep.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daria6918.cn/gtpazqhaya.html

[R76] 使用临时文件
来源：http://hz.jlsjyb.cn/gtrsmgljwd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gthcveiufg.html

[R77] 读取用户输入
来源：http://hz.fzhhl.top/gtqkxmperu.html

read -rp "请输入: " ans
来源：http://hz.jinyuanbaomall.cn/gtixxggput.html

[R78] 交互式菜单
来源：http://hz.ybcxt.top/gtfktwoqba.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shuidangran.top/gtjawvxamb.html

[R79] 解析命令行选项
来源：http://hz.aibaodan.cn/gtktwuuszq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.birdmap.top/gthlricrgw.html

[R80] 查看脚本执行耗时
来源：http://hz.yj20258888.top/gtjfzqxoer.html

time ./run.sh
来源：http://hz.jyoumei.cn/gtwmutkslw.html

================================================================================
来源：http://hz.bjfxy.top/gtcfbnqllo.html

S. C / C++ 专题
来源：http://hz.birdmap.top/gtmodclamc.html

================================================================================
来源：http://hz.smart0.xyz/gtdqlicojk.html

[S01] C：Hello World
来源：http://hz.c1oappe.top/gtoohktact.html

#include <stdio.h>
来源：http://hz.ybcxt.top/gtqavkdykw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cucudq.cn/gtucypnkqq.html

[S02] C：变量与格式化输出
来源：http://hz.xziqi.cn/gtwwzwqaie.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuxming.cn/gtbkzkenpc.html

[S03] C：读入整数
来源：http://hz.yj20258.top/gtgurdihct.html

int x; scanf("%d", &x);
来源：http://hz.sxryk.cn/gtzycuhatu.html

[S04] C：字符串复制
来源：http://hz.sufxvd.cn/gtxynsccqz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gttcvftlxk.html

[S05] C：字符串长度
来源：http://hz.svipenyu.cn/gtsuhnfnav.html

strlen(s)
来源：http://hz.yueranfly.top/gtgqkyxprj.html

[S06] C：字符串比较
来源：http://hz.daxiang520.top/gtwylbnyku.html

strcmp(a, b) == 0
来源：http://hz.redwolf501.top/gtovnyiwvn.html

[S07] C：数组遍历求和
来源：http://hz.aizwys.cn/gtgolfdyfw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cucudq.cn/gtisnjcquw.html

[S08] C：动态内存分配与释放
来源：http://hz.kuanghao11.cn/gtbppyjgaj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yonumen.top/gtemykapln.html

[S09] C：结构体定义与初始化
来源：http://hz.havefunace.top/gtnjbedrem.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sufxvd.cn/gttqcetatf.html

[S10] C：指针与解引用
来源：http://hz.tian-w.cn/gtqatqfgqo.html

int *p = &a;  *p = 5;
来源：http://hz.zhijiandao.cn/gtgwfefxkj.html

[S11] C：逐行读文件
来源：http://hz.jiagoushi.top/gtzfzyfgdg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cucudq.cn/gttzinfmkn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.redwolf501.top/gtklqdhysl.html

fclose(f);
来源：http://hz.hammf.cn/gteqxndpxy.html

[S12] C：写文件
来源：http://hz.ydzc1.top/gtqmykqcei.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ywan-chungtsiang.top/gthllqwetl.html

[S13] C：宏定义
来源：http://hz.hnqzz.top/gtssuhofxz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cdnleiting.top/gtibfmcenz.html

[S14] C：枚举
来源：http://hz.ybcxt.top/gtgiwjvied.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nanxuanxn.top/gtedaasjbd.html

[S15] C：类型转换
来源：http://hz.jyoumei.cn/gtopwvsixf.html

(double) a / b
来源：http://hz.sufxvd.cn/gttzzganox.html

[S16] C：位操作置位
来源：http://hz.cashguo.top/gtmxqmkeva.html

x |= (1 << 3);
来源：http://hz.yj202588.top/gtwqzmmwvu.html

[S17] C：安全拼接字符串
来源：http://hz.jqgfzy.top/gtfrbypnfg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gotoacloud.top/gtehhyxfqs.html

[S18] C：命令行参数
来源：http://hz.52xcode.cn/gtoafakoda.html

int main(int argc, char **argv)
来源：http://hz.ydzc1.top/gtdbwjfifz.html

[S19] C：快速排序
来源：http://hz.xylfe.cn/gttqarmmon.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sxryk.cn/gtvmeugbrv.html

[S20] C：二分查找
来源：http://hz.tian-w.cn/gtfxttschs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.vqdsnc.cn/gtklmdxqnv.html

[S21] C：字符类别判断
来源：http://hz.yj20258.top/gthaqgkwrl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shanyushiyangkeji.top/gtlmuobftg.html

[S22] C：字符串转数字
来源：http://hz.fzhhl.top/gtugmaabxc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.9152youxi.cn/gtflduhtmb.html

[S23] C：随机数
来源：http://hz.zhijiandao.cn/gtwvgkrhbz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zycfv.cn/gtofxgvemt.html

[S24] C：获取本地时间
来源：http://hz.ywan-chungtsiang.top/gtbmnipaby.html


<!-- 参考信息 -->