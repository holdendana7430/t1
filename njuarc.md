代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.redwolf501.top/gtzwllqczl.html

[Q58] 累计求和
来源：http://hz.hnxiangtu.top/gtmutqtors.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sysykeji.top/gtiscadmrw.html

[Q59] 分组内累计
来源：http://hz.zycfv.cn/gtarvepnpq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.iojbl.cn/gtzpcyvvnj.html

[Q60] 取上一行 / 下一行
来源：http://hz.pengpengdd.cyou/gtesalmeez.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xziqi.cn/gtdrjbhhwv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.havefunace.top/gtjtskvebr.html

[Q61] 移动平均
来源：http://hz.yonumen.top/gtefmgkefz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.fengsongda.top/gtbqbeklvt.html

[Q62] 分组占比
来源：http://hz.jiagoushi.top/gtbbbfoenw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtlrrspeia.html

[Q63] 开启事务
来源：http://hz.52xcode.cn/gtgcduljgs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.havefunace.top/gtjtreyxed.html

[Q64] 提交事务
来源：http://hz.yj202588.top/gtrkmqnaun.html

COMMIT;
来源：http://hz.xylfe.cn/gtfrwjlebs.html

[Q65] 回滚事务
来源：http://hz.bjfxy.top/gtdrcaujte.html

ROLLBACK;
来源：http://hz.yongpay.top/gtfdocjyxr.html

[Q66] 行锁查询
来源：http://hz.zhoulong.xyz/gtzielkobb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhixingplan.top/gtttctfcjz.html

[Q67] 设置隔离级别
来源：http://hz.meibo888.top/gthpzgjuqd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zdqjudy.top/gtuhpxfnkv.html

[Q68] 保存点
来源：http://hz.zhoulong.xyz/gtlbhifnhv.html

SAVEPOINT sp1;
来源：http://hz.svipenyu.cn/gtqvwnhlln.html

ROLLBACK TO sp1;
来源：http://hz.9152youxi.cn/gthpnlgdzt.html

[Q69] 查看执行计划
来源：http://hz.nwbrower.top/gtennsmzbj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hysaishi.cn/gtbpqyrvze.html

[Q70] 更新统计信息
来源：http://hz.hfpthk.cn/gtkzuqodtc.html

ANALYZE TABLE users;
来源：http://hz.chenjidiqi.icu/gtqsewqoac.html

[Q71] 查看建表语句
来源：http://hz.snrcjt.cn/gtafzfxspc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hywenlv.cn/gtnvizhhsu.html

[Q72] 查看索引
来源：http://hz.feifeiyinyue.top/gtowkkwjjg.html

SHOW INDEX FROM users;
来源：http://hz.tian-w.cn/gtbplqekts.html

[Q73] 查看表状态
来源：http://hz.shzxlz.cn/gtweclckjs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ivvv.top/gttahnnsls.html

[Q74] 强制使用索引
来源：http://hz.hnqzz.top/gtpmukibtp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xingfuxueyuan.xyz/gtfhvgsmyi.html

[Q75] 日期格式化
来源：http://hz.zhijiandao.cn/gttjiptrwv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuanzhike.top/gtqwcqrfhj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jyoumei.cn/gtedgltvmp.html

[Q76] 按天统计
来源：http://hz.nwbrower.top/gtdnotgwxv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenlongwang.top/gtmionumrj.html

[Q77] 时间加减
来源：http://hz.jlsjyb.cn/gtnxjbbzvq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.redwolf501.top/gtozdyeldg.html

[Q78] 当前时间
来源：http://hz.yueranfly.top/gtobfsfqms.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxuanxn.top/gtiukosvqu.html

[Q79] 字符串拼接
来源：http://hz.ydjk.org.cn/gtfnaniomz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jianghu66.top/gtbtrejxvz.html

[Q80] 字符串截取
来源：http://hz.shanyushiyangtech.top/gtkjhcsrot.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinqigfzy.top/gtrggwurmt.html

[Q81] 字符串替换
来源：http://hz.guowangkeji.top/gtctarsmcc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.aibaodan.cn/gtuptkbqtd.html

[Q82] 字符长度与字节长度
来源：http://hz.shanyushiyangtech.top/gtzkiircwi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hywenlv.cn/gtfiebanqn.html

[Q83] 大小写转换
来源：http://hz.svipenyu.cn/gtcugcdyow.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.bjfxy.top/gtthzqxaot.html

[Q84] 去除首尾空格
来源：http://hz.guowangkeji.top/gtfizaotxq.html

SELECT TRIM(name) FROM users;
来源：http://hz.guannengcc.top/gtlwlcdxup.html

[Q85] 数值取整
来源：http://hz.gogol.net.cn/gtjmbcsrro.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xziqi.cn/gtadnzlwhk.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigfzy.top/gtmzxxfejo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hongshengwenyu.top/gtnaneospq.html

[Q87] JSON 字段做条件
来源：http://hz.pycfn.com/gtdiukklac.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.redwolf501.top/gtqheruikx.html

[Q88] 行转列（条件聚合）
来源：http://hz.xinyue.icu/gtpxfstdpt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.iojbl.cn/gtumjwgapx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.aibaodan.cn/gtjeviyfhb.html

[Q89] 判断表是否存在
来源：http://hz.aibaodan.cn/gtjivolyvh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nwbrower.top/gtaabgwtxp.html

[Q90] 生成序号列
来源：http://hz.meibo888.top/gtvwszifma.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jqgfzy.top/gtfpnqfgrl.html

================================================================================
来源：http://hz.9152youxi.cn/gtqvvhludi.html

R. Bash 专题
来源：http://hz.sxryk.cn/gtelravxzi.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtqgmvsrtr.html

[R01] shebang 与严格模式
来源：http://hz.feifeiyinyue.top/gtjcbfjvxx.html

#!/usr/bin/env bash
来源：http://hz.cashguo.top/gtwkwqsbpk.html

set -euo pipefail
来源：http://hz.ivvv.top/gtryhjxyoe.html

[R02] 变量赋值与使用
来源：http://hz.nanxinkj.top/gtowsshafw.html

name="Tom"; echo "$name"
来源：http://hz.hysaishi.cn/gtbqfoufmh.html

[R03] 只读变量
来源：http://hz.hnqzz.top/gtgddhhfwr.html

readonly PI=3.14
来源：http://hz.ehwqpu.com/gtjysmvdlq.html

[R04] 位置参数
来源：http://hz.gotoacloud.top/gtkquxnfni.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ywan-chungtsiang.top/gtkmzcvshp.html

[R05] 参数默认值
来源：http://hz.haohaochexian.top/gtbssygkpv.html

name="${1:-default}"
来源：http://hz.zhijiandao.cn/gtncxxflql.html

[R06] 判断命令是否存在
来源：http://hz.meibo888.top/gtrkovscar.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhaomingkeji.xyz/gttepzecto.html

[R07] if 判断文件
来源：http://hz.hnqzz.top/gtdbvomtyw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yongpay.top/gtjnolozei.html

[R08] 数值比较
来源：http://hz.jlsjyb.cn/gtyhvotamb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.fzhhl.top/gtinnnhwdm.html

[R09] 字符串比较
来源：http://hz.sufxvd.cn/gtdyidwqlk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.daria6918.cn/gtacuirpir.html

[R10] 正则匹配
来源：http://hz.yvedp.cn/gtukjmtcjk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtsvdfekjt.html

[R11] case 多分支
来源：http://hz.yongpay.top/gtusfaqoyc.html

case "$1" in
来源：http://hz.jqgfzy.top/gtynfxpkvg.html

start) echo "启动" ;;
来源：http://hz.hnqzz.top/gtwdhzklrk.html

stop)  echo "停止" ;;
来源：http://hz.xuanzx.com/gtawurqskl.html

*)     echo "未知命令" ;;
来源：http://hz.gogol.net.cn/gtpizdriaf.html

esac
来源：http://hz.hammf.cn/gtaukradzr.html

[R12] for 遍历文件
来源：http://hz.hongshengwenyu.top/gtgtkzkrno.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhengqikj.top/gtjllbfsgp.html

[R13] for 计数循环
来源：http://hz.nwbrower.top/gtvvofgdye.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtkexlvsrd.html

[R14] C 风格 for
来源：http://hz.0kj1m.cn/gtezyoedne.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ybcxt.top/gtcwvzzvnu.html

[R15] while 逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtxuosjahh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yongpay.top/gtpmupmfca.html

[R16] until 等待条件
来源：http://hz.gaohongyu789.top/gthiivqjpv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.guowangkeji.top/gtikresgnw.html

[R17] 数组定义与取值
来源：http://hz.yj20258888.top/gtzkospgdz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xziqi.cn/gtcnuqabnc.html

[R18] 遍历数组
来源：http://hz.ydzc1.top/gtxonuqdkc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinqigufen.top/gtdoshmdkt.html

[R19] 数组长度
来源：http://hz.birdmap.top/gtrzeetiah.html

echo "${#arr[@]}"
来源：http://hz.gotoacloud.top/gtiysjkqdt.html

[R20] 关联数组（字典）
来源：http://hz.cqqwz.cn/gtzyxitdqh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangtech.top/gtssdkggqb.html

[R21] 字符串长度
来源：http://hz.mhx1999.top/gthtjwbnsr.html

echo "${#s}"
来源：http://hz.xylfe.cn/gthxxuloiu.html

[R22] 截取子串
来源：http://hz.cqqwz.cn/gtfdvnjext.html

echo "${s:0:5}"
来源：http://hz.yangfankeji.com/gtxbovgxuc.html

[R23] 字符串替换
来源：http://hz.yj20258.top/gtrcygdgsn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.tanke756.top/gtbattnhbk.html

[R24] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtbfeqoilm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tanke756.top/gtknkxdbai.html

[R25] 去后缀 / 去前缀
来源：http://hz.9152youxi.cn/gtiqsvttkc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hysaishi.cn/gttbmrpzel.html

[R26] 命令替换
来源：http://hz.svipenyu.cn/gtbjbxxedc.html

now=$(date +%F); echo "$now"
来源：http://hz.jlsjyb.cn/gtlvlxghyy.html

[R27] 算术展开
来源：http://hz.jlsjyb.cn/gtfnvhqesw.html

echo $((1 + 2 * 3))
来源：http://hz.iojbl.cn/gtcbfxdeny.html

[R28] 浮点运算
来源：http://hz.dashuyun.cn/gtljvhldjp.html

echo "scale=2; 10/3" | bc
来源：http://hz.yuxming.cn/gtlzfcttzd.html

[R29] 定义函数
来源：http://hz.gotoacloud.top/gttlxxdjyb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.daxiang520.top/gtulpwjlvl.html

[R30] 函数返回状态码
来源：http://hz.hfpthk.cn/gtcpojybnx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.iojbl.cn/gtpvuqspjf.html

[R31] 局部变量
来源：http://hz.xuanzx.com/gtohssvnkv.html

f() { local x=1; echo "$x"; }
来源：http://hz.gotoacloud.top/gtfqhkzxje.html

[R32] 参数个数校验
来源：http://hz.smart0.xyz/gtssebagya.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yvedp.cn/gtujnxfkma.html

[R33] 捕获错误并提示行号
来源：http://hz.ivvv.top/gtguccxcex.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yonumen.top/gtrrntbhmq.html

[R34] 退出时清理
来源：http://hz.pengpengdd.cyou/gtcjmhcvwa.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hammf.cn/gtpoohkbfz.html

[R35] 后台执行并等待
来源：http://hz.gotoacloud.top/gthkzmzbyv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.nwbrower.top/gtegsgyrml.html

[R36] 并发执行多个任务
来源：http://hz.daria6918.cn/gtcuhorsxj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cheryme.top/gtrpdgobyv.html

[R37] 把输出赋给变量
来源：http://hz.hnxiangtu.top/gthkouvyvw.html

files=$(ls -1)
来源：http://hz.gotoacloud.top/gtysskarmh.html

[R38] 管道串联
来源：http://hz.snrcjt.cn/gtkzganrgf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cashguo.top/gtjxzuhwpo.html

[R39] 重定向标准输出与错误
来源：http://hz.vqdsnc.cn/gtzrxqozsy.html

cmd > out.log 2>&1
来源：http://hz.0kj1m.cn/gtvfhxrldq.html

[R40] 追加写日志
来源：http://hz.xuanzx.com/gtajdvbgck.html

echo "log" >> out.log
来源：http://hz.tianlin.xyz/gthachtkvq.html

[R41] 丢弃输出
来源：http://hz.cqqwz.cn/gtizvudmuw.html

cmd >/dev/null 2>&1
来源：http://hz.fengsongda.top/gtfguydvtu.html

[R42] 输入重定向
来源：http://hz.snrcjt.cn/gtznklhucu.html

wc -l < a.txt
来源：http://hz.zycfv.cn/gtjjuezyqu.html

[R43] 按名字查找文件
来源：http://hz.iojbl.cn/gtwmtmpslb.html

find . -name "*.log" -type f
来源：http://hz.shzxlz.cn/gttjggnziz.html

[R44] 按修改时间查找
来源：http://hz.yueranfly.top/gtjobomwbv.html

find . -mtime -7 -type f
来源：http://hz.pycfn.com/gtfohiaohs.html

[R45] 批量删除
来源：http://hz.gaohongyu789.top/gtjjokvukw.html

find . -name "*.tmp" -delete
来源：http://hz.jqgfzy.top/gtbxtljspt.html

[R46] 递归替换文件内容
来源：http://hz.jqgufenzy.top/gtpcrduwwc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.316326.xyz/gthsdpidxf.html

[R47] sed 单行替换
来源：http://hz.ywan-chungtsiang.top/gtrhkkvqrm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.c1oappe.top/gtojnpyjlw.html

[R48] awk 取指定列
来源：http://hz.jqgfzy.top/gtenfpgmse.html

awk '{print $1, $3}' a.txt
来源：http://hz.yvedp.cn/gtmogxspau.html

[R49] awk 带条件
来源：http://hz.jlsjyb.cn/gtolwlqcpz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhengqikj.top/gtlzfcjhqh.html

[R50] awk 求和
来源：http://hz.zhaomingkeji.xyz/gtvzeizezg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shanyushiyangtech.top/gtwfdkpruz.html

[R51] 排序去重取前几
来源：http://hz.316326.xyz/gtjqvilnmg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydjk.org.cn/gtotslrxgh.html

[R52] 统计行数
来源：http://hz.jqgufenzy.top/gtkzgegjko.html

wc -l a.txt
来源：http://hz.yj20258.top/gtjyxabwgg.html

[R53] 查看文件头与实时尾
来源：http://hz.jyoumei.cn/gtkxfeuefw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shuidangran.top/gtfreaatoh.html

[R54] 比较两个文件
来源：http://hz.zhoulong.xyz/gtzkwhoquf.html

diff a.txt b.txt
来源：http://hz.jqgufenzy.top/gthyiioxfo.html

[R55] 压缩与解压
来源：http://hz.hnqzz.top/gtxemcbhic.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigfzy.top/gtlzvvuodj.html

[R56] 远程拷贝
来源：http://hz.vqdsnc.cn/gtpeynvyhu.html

scp file user@host:/path/
来源：http://hz.zhoulong.xyz/gtvtctifxz.html

[R57] 远程执行命令
来源：http://hz.yonumen.top/gtssasfmvi.html

ssh user@host 'uptime'
来源：http://hz.yj20258888.top/gtxqmhvlro.html

[R58] 下载文件
来源：http://hz.shangyingyoupin.top/gtrflnlugc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xinyue.icu/gttbwdnjea.html

[R59] 发 POST JSON
来源：http://hz.hywenlv.cn/gtmraxsoxd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yanxiufei.cn/gtzivaovvl.html

[R60] 只看 HTTP 状态码
来源：http://hz.hammf.cn/gtvzaxiqwv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhiwuduotai.top/gteetqghld.html

[R61] 磁盘占用
来源：http://hz.haohaochexian.top/gtbfvncdhc.html

df -h;  du -sh *
来源：http://hz.yvedp.cn/gtdixczkwr.html

[R62] 找最占空间的文件
来源：http://hz.iojbl.cn/gthvkvsyvi.html

du -ah . | sort -rh | head -10
来源：http://hz.svipenyu.cn/gtaudxjwqt.html

[R63] 内存与进程
来源：http://hz.316326.xyz/gtefbgbndt.html

free -h;  ps aux | grep nginx
来源：http://hz.yvedp.cn/gtjwpgqxrc.html

[R64] 结束进程
来源：http://hz.fzhhl.top/gtimyasbpu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xuanzx.com/gtktgnqbuz.html

[R65] 查看端口占用
来源：http://hz.cheryme.top/gtmtrgzcql.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aibaodan.cn/gtmutuoslc.html

[R66] 定时任务
来源：http://hz.xinyue.icu/gtqlrhmens.html

crontab -e;  crontab -l
来源：http://hz.yangfankeji.com/gtmuvlntor.html

[R67] 生成随机十六进制串
来源：http://hz.yuxming.cn/gtdlyompdk.html

openssl rand -hex 16
来源：http://hz.fengsongda.top/gtcvexpzgl.html

[R68] 计算文件校验值
来源：http://hz.52xcode.cn/gtskeuqhni.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.snrcjt.cn/gtrtjnmsoe.html

[R69] 生成随机密码
来源：http://hz.tanke756.top/gtuxjitlil.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhongyouzk.top/gtcwgmziiw.html

[R70] 时间戳与互转
来源：http://hz.zhijiandao.cn/gtwpvjylab.html

date +%s;  date -d @1700000000
来源：http://hz.wangdashe.top/gtzbsjfsjo.html

[R71] 日期格式化
来源：http://hz.zhaomingkeji.xyz/gthtkddzem.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nwbrower.top/gtgncufatc.html

[R72] 等待端口就绪
来源：http://hz.zhongyouzk.top/gtjaydvner.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.wangdashe.top/gtcslzhgpq.html

[R73] 分割大日志
来源：http://hz.shuidangran.top/gtwzgwbcdw.html

split -l 1000 big.log part_
来源：http://hz.gaohongyu789.top/gtlnhfgtch.html

[R74] 批量重命名
来源：http://hz.chenzaomai.com/gtpltrdrdn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinyuanbaomall.cn/gtnwwjuriu.html

[R75] 导出环境变量
来源：http://hz.meibo888.top/gtkfrnzgwf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.haohaochexian.top/gtiijqdknh.html

[R76] 使用临时文件
来源：http://hz.iojbl.cn/gtopbznchf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtiaqjemac.html

[R77] 读取用户输入
来源：http://hz.zhijiandao.cn/gtukeapbqk.html

read -rp "请输入: " ans
来源：http://hz.shuidangran.top/gtpeqfkcqy.html

[R78] 交互式菜单
来源：http://hz.tianlin.xyz/gtwxajvros.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnqzz.top/gtkcuqoydq.html

[R79] 解析命令行选项
来源：http://hz.nwbrower.top/gtlxmweghs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ppjwa.cn/gtlpwjxolj.html

[R80] 查看脚本执行耗时
来源：http://hz.xylfe.cn/gtdxiuyfcz.html

time ./run.sh
来源：http://hz.yuanzhike.top/gtgxschwth.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtreakausl.html

S. C / C++ 专题
来源：http://hz.cheryme.top/gtfmdjatar.html

================================================================================
来源：http://hz.sxryk.cn/gtlpyhjybb.html

[S01] C：Hello World
来源：http://hz.sysykeji.top/gtuecyczfs.html

#include <stdio.h>
来源：http://hz.yuxming.cn/gtcnhlmpif.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yonumen.top/gtokeiwfgg.html

[S02] C：变量与格式化输出
来源：http://hz.tian-w.cn/gtbyjjutlr.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenjidiqi.icu/gttgrinbpz.html

[S03] C：读入整数
来源：http://hz.guowangkeji.top/gtabwbzjli.html

int x; scanf("%d", &x);
来源：http://hz.zhengqikj.top/gtqfatxmns.html

[S04] C：字符串复制
来源：http://hz.shanyushiyangtech.top/gthignkqwa.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydjk.org.cn/gtmlgoijwb.html

[S05] C：字符串长度
来源：http://hz.ywan-chungtsiang.top/gtnelsxyww.html

strlen(s)
来源：http://hz.zhixingplan.top/gtacjpeqwv.html

[S06] C：字符串比较
来源：http://hz.ywan-chungtsiang.top/gtutougwmx.html

strcmp(a, b) == 0
来源：http://hz.zhoulong.xyz/gtwxmusibd.html

[S07] C：数组遍历求和
来源：http://hz.zhengqikj.top/gtzjekrrmo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shanyushiyangkeji.top/gtdrnjpxzm.html

[S08] C：动态内存分配与释放
来源：http://hz.hysaishi.cn/gtooqdokmm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hongshengwenyu.top/gtfwnxafpu.html

[S09] C：结构体定义与初始化
来源：http://hz.yanxiufei.cn/gtztojylyz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cashguo.top/gtstxmrnjf.html

[S10] C：指针与解引用
来源：http://hz.chenjidiqi.icu/gtuyjrzoft.html

int *p = &a;  *p = 5;
来源：http://hz.zdqjudy.top/gtbdkcsrrr.html

[S11] C：逐行读文件
来源：http://hz.ydzc1.top/gtsbhrrzrm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yueranfly.top/gtsqnxxinb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.pycfn.com/gtqjtpfvma.html

fclose(f);
来源：http://hz.sweek.top/gtvsneejfr.html

[S12] C：写文件
来源：http://hz.gogol.net.cn/gtcuarrbsw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yuanzhike.top/gtkymdgzvm.html

[S13] C：宏定义
来源：http://hz.9152youxi.cn/gteavviltn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.redwolf501.top/gtomrvyimh.html

[S14] C：枚举
来源：http://hz.hammf.cn/gteclkguwu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj202588.top/gtvaysgubc.html

[S15] C：类型转换
来源：http://hz.sweek.top/gtmvfhwevz.html

(double) a / b
来源：http://hz.shzxlz.cn/gtstmxlhjd.html

[S16] C：位操作置位
来源：http://hz.zhoulong.xyz/gtonnavuxr.html

x |= (1 << 3);
来源：http://hz.jinghuilouyu.cn/gthjvcaewl.html

[S17] C：安全拼接字符串
来源：http://hz.ybcxt.top/gtnjmwuhfs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgfzy.top/gtyjrugort.html

[S18] C：命令行参数
来源：http://hz.xingfuxueyuan.xyz/gtktzkjfzz.html

int main(int argc, char **argv)
来源：http://hz.jqgfzy.top/gtmfwpicsp.html

[S19] C：快速排序
来源：http://hz.chenzaomai.com/gtkwgodmis.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtlzfpablt.html

[S20] C：二分查找
来源：http://hz.shangyingyoupin.top/gtjqoflbqp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hammf.cn/gtteclfvhk.html

[S21] C：字符类别判断
来源：http://hz.yangfankeji.com/gtiscvcdpj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhongyouzk.top/gtzcdyfxxg.html

[S22] C：字符串转数字
来源：http://hz.yueranfly.top/gtlwgidqcl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj20258888.top/gtsrjhdbje.html

[S23] C：随机数
来源：http://hz.yvedp.cn/gtlwtitkxj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinqigufen.top/gtgxpqduva.html

[S24] C：获取本地时间
来源：http://hz.haohaochexian.top/gtwmggpwqw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dashuyun.cn/gtpstpghhf.html

[S25] C：内存拷贝
来源：http://hz.yonumen.top/gtglwfthih.html

memcpy(dst, src, n);
来源：http://hz.cashguo.top/gtjlmntulo.html

[S26] C：内存清零
来源：http://hz.yongpay.top/gtskzsadtv.html

memset(a, 0, sizeof a);
来源：http://hz.bjfxy.top/gthkkywrgd.html

[S27] C：定义常量
来源：http://hz.yuanzhike.top/gtvznblhsp.html

const double PI = 3.14159;
来源：http://hz.ydjk.org.cn/gtozjdbilo.html

[S28] C：静态变量
来源：http://hz.zhoulong.xyz/gtekspnfbe.html


<!-- 参考信息 -->