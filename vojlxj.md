代发 wailian999

[Q61] 移动平均
来源：http://hz.cheryme.top/gtvhqnzdbv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.haohaochexian.top/gtgacztdlc.html

[Q62] 分组占比
来源：http://hz.sxryk.cn/gtwcrhwytx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtydcefaci.html

[Q63] 开启事务
来源：http://hz.fengsongda.top/gtfmuogibx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xuetiantiany.cn/gtlpcojcbe.html

[Q64] 提交事务
来源：http://hz.nanxuanxn.top/gtxszofdws.html

COMMIT;
来源：http://hz.jyoumei.cn/gtnpflhuiu.html

[Q65] 回滚事务
来源：http://hz.jqgufenzy.top/gtcwissskq.html

ROLLBACK;
来源：http://hz.fengsongda.top/gtqbnnqljo.html

[Q66] 行锁查询
来源：http://hz.feifeiyinyue.top/gtabcenlcm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zdqjudy.top/gtrrarvjiw.html

[Q67] 设置隔离级别
来源：http://hz.sweek.top/gtizfxvegp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cdnleiting.top/gtymorawdc.html

[Q68] 保存点
来源：http://hz.jqgufenzy.top/gtnfyrbxps.html

SAVEPOINT sp1;
来源：http://hz.ydjk.org.cn/gtrhmccbeg.html

ROLLBACK TO sp1;
来源：http://hz.havefunace.top/gtblmqybvi.html

[Q69] 查看执行计划
来源：http://hz.cqqwz.cn/gtkmcomzkf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tian-w.cn/gtjmmuckkt.html

[Q70] 更新统计信息
来源：http://hz.zhengqikj.top/gtmghdhiaq.html

ANALYZE TABLE users;
来源：http://hz.fengsongda.top/gtohtbtemi.html

[Q71] 查看建表语句
来源：http://hz.yonumen.top/gtxmxmyshx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenlongwang.top/gtdndzsyxv.html

[Q72] 查看索引
来源：http://hz.xziqi.cn/gtgoowslmw.html

SHOW INDEX FROM users;
来源：http://hz.yonumen.top/gtpudfzybz.html

[Q73] 查看表状态
来源：http://hz.chenlongwang.top/gtkrxqvccn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nwbrower.top/gtiuoujmzx.html

[Q74] 强制使用索引
来源：http://hz.zycfv.cn/gtwaldxtdz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shanyushiyangtech.top/gtygdegaxm.html

[Q75] 日期格式化
来源：http://hz.jyoumei.cn/gtcloegpqt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuxming.cn/gttfopnlzm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yuanzhike.top/gtayukdvjk.html

[Q76] 按天统计
来源：http://hz.zhongyouzk.top/gtmxwzouwk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.meibo888.top/gtnejxrfsz.html

[Q77] 时间加减
来源：http://hz.hnxiangtu.top/gtgqylxcln.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fengsongda.top/gtzgfxbfwq.html

[Q78] 当前时间
来源：http://hz.sysykeji.top/gtlpfurjgg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shangyingyoupin.top/gtpquplmhy.html

[Q79] 字符串拼接
来源：http://hz.xziqi.cn/gtpqiubikq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.quarkkingdee.top/gtpcenlabu.html

[Q80] 字符串截取
来源：http://hz.daxiang520.top/gtlwcuukbl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cucudq.cn/gtliskqgxs.html

[Q81] 字符串替换
来源：http://hz.ybcxt.top/gtjhrixmha.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.mhx1999.top/gtyudbiuje.html

[Q82] 字符长度与字节长度
来源：http://hz.gaohongyu789.top/gtiftrilby.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yangfankeji.com/gtumcffiem.html

[Q83] 大小写转换
来源：http://hz.quarkkingdee.top/gtkhyakjsh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.vqdsnc.cn/gtpzogtbmj.html

[Q84] 去除首尾空格
来源：http://hz.xuetiantiany.cn/gtnfbzewej.html

SELECT TRIM(name) FROM users;
来源：http://hz.yueranfly.top/gtxxfbrgeq.html

[Q85] 数值取整
来源：http://hz.ydjk.org.cn/gtfziscrrr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.bjfxy.top/gtqqsocnya.html

[Q86] 读取 JSON 字段
来源：http://hz.zhijiandao.cn/gtiblgiowv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinqigufen.top/gtvgqwsqqi.html

[Q87] JSON 字段做条件
来源：http://hz.yvedp.cn/gtfzvheqfc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.fzhhl.top/gtaqpvfygd.html

[Q88] 行转列（条件聚合）
来源：http://hz.sxryk.cn/gtzlfzeotn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.wangdashe.top/gtchnnofql.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sweek.top/gtgnphmpke.html

[Q89] 判断表是否存在
来源：http://hz.hnqzz.top/gtnjgagkfc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.birdmap.top/gtgllhcpke.html

[Q90] 生成序号列
来源：http://hz.yj20258888.top/gtsvhwcxaj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pycfn.com/gtbfbmucdo.html

================================================================================
来源：http://hz.daxiang520.top/gtqnbptjkz.html

R. Bash 专题
来源：http://hz.0kj1m.cn/gtoxdzhkkr.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtnidveksl.html

[R01] shebang 与严格模式
来源：http://hz.jinyuanbaomall.cn/gtyrbwqnew.html

#!/usr/bin/env bash
来源：http://hz.yongpay.top/gtemafsmgm.html

set -euo pipefail
来源：http://hz.shanyushiyangkeji.top/gtbqbllvsa.html

[R02] 变量赋值与使用
来源：http://hz.hysaishi.cn/gtheppkqsq.html

name="Tom"; echo "$name"
来源：http://hz.yuanzhike.top/gthbaihwta.html

[R03] 只读变量
来源：http://hz.shanyushiyangkeji.top/gtedydkozx.html

readonly PI=3.14
来源：http://hz.cdnleiting.top/gtaewcboba.html

[R04] 位置参数
来源：http://hz.xylfe.cn/gtdbxhyqsh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhaomingkeji.xyz/gtfrrdxzde.html

[R05] 参数默认值
来源：http://hz.sxryk.cn/gtcygxjmef.html

name="${1:-default}"
来源：http://hz.zhiwuduotai.top/gtcorwkzsy.html

[R06] 判断命令是否存在
来源：http://hz.jinqigufen.top/gtqiansjxn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj202588.top/gtpbvzeply.html

[R07] if 判断文件
来源：http://hz.daria6918.cn/gtrxvgxqsw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.vqdsnc.cn/gtizeakgli.html

[R08] 数值比较
来源：http://hz.dashuyun.cn/gtrprumnfn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nwbrower.top/gtuigftuqb.html

[R09] 字符串比较
来源：http://hz.cashguo.top/gtepuwrrez.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hnqzz.top/gtjmkkjnyi.html

[R10] 正则匹配
来源：http://hz.zhoulong.xyz/gttrndiddj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tianlin.xyz/gtvnnrzaxh.html

[R11] case 多分支
来源：http://hz.gaohongyu789.top/gtpbjgmffc.html

case "$1" in
来源：http://hz.shanyushiyangkeji.top/gtqjonecqd.html

start) echo "启动" ;;
来源：http://hz.tianlin.xyz/gtyjtnprbk.html

stop)  echo "停止" ;;
来源：http://hz.yueranfly.top/gtgvawscot.html

*)     echo "未知命令" ;;
来源：http://hz.cqqwz.cn/gtimgpherd.html

esac
来源：http://hz.svipenyu.cn/gtnundgoqk.html

[R12] for 遍历文件
来源：http://hz.bjfxy.top/gtcfqynodx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nanxuanxn.top/gtexwnryav.html

[R13] for 计数循环
来源：http://hz.xylfe.cn/gtauvneglw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtyoypbdby.html

[R14] C 风格 for
来源：http://hz.jinghuilouyu.cn/gtfvynvdde.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinqigufen.top/gtetryuwtj.html

[R15] while 逐行读文件
来源：http://hz.jyoumei.cn/gtdkdadndo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hnxiangtu.top/gtglfpwcis.html

[R16] until 等待条件
来源：http://hz.jlsjyb.cn/gtbbrjuzcj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhoulong.xyz/gtoxmmfsva.html

[R17] 数组定义与取值
来源：http://hz.xziqi.cn/gtonbhdgfq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nanxinkj.top/gtkwmrzsog.html

[R18] 遍历数组
来源：http://hz.jianghu66.top/gtcexxgltl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgfzy.top/gtvpowoiiz.html

[R19] 数组长度
来源：http://hz.snrcjt.cn/gtccwodbvq.html

echo "${#arr[@]}"
来源：http://hz.yonumen.top/gtcpiedwdb.html

[R20] 关联数组（字典）
来源：http://hz.hnqzz.top/gtksrtcdcs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shangyingyoupin.top/gtslxmuejk.html

[R21] 字符串长度
来源：http://hz.gogol.net.cn/gtjiyyvoqo.html

echo "${#s}"
来源：http://hz.ywan-chungtsiang.top/gtnjtkalpj.html

[R22] 截取子串
来源：http://hz.zhengqikj.top/gtyrerbjnc.html

echo "${s:0:5}"
来源：http://hz.jinyuanbaomall.cn/gtxrizddbg.html

[R23] 字符串替换
来源：http://hz.gzhubu.top/gtnbifavyb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shangyingyoupin.top/gtcccthbda.html

[R24] 大小写转换
来源：http://hz.yuxming.cn/gtytzngmkw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhaomingkeji.xyz/gtowwfmxcy.html

[R25] 去后缀 / 去前缀
来源：http://hz.bjfxy.top/gtsivmquvm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gotoacloud.top/gttwkibabd.html

[R26] 命令替换
来源：http://hz.ywan-chungtsiang.top/gtuvvdpask.html

now=$(date +%F); echo "$now"
来源：http://hz.316326.xyz/gtcwyghqev.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gtyfjleuqy.html

echo $((1 + 2 * 3))
来源：http://hz.52xcode.cn/gtzaxpoibd.html

[R28] 浮点运算
来源：http://hz.jiagoushi.top/gtwtsaerqq.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj20258.top/gtsornnwnl.html

[R29] 定义函数
来源：http://hz.jyoumei.cn/gtozbmgibk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhixingplan.top/gtvipgmajk.html

[R30] 函数返回状态码
来源：http://hz.zdqjudy.top/gthunomzap.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pengpengdd.cyou/gtxzxmmjpj.html

[R31] 局部变量
来源：http://hz.xingfuxueyuan.xyz/gtuawqrbip.html

f() { local x=1; echo "$x"; }
来源：http://hz.jiagoushi.top/gtcqymjcof.html

[R32] 参数个数校验
来源：http://hz.fengsongda.top/gtuhucsunh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ydjk.org.cn/gtyyjllmfd.html

[R33] 捕获错误并提示行号
来源：http://hz.zhaomingkeji.xyz/gtuoqhvywk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.redwolf501.top/gthglhjuvy.html

[R34] 退出时清理
来源：http://hz.yonumen.top/gtbnxwhrmx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jlsjyb.cn/gtrvescpjm.html

[R35] 后台执行并等待
来源：http://hz.shzxlz.cn/gtchoubrha.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.c1oappe.top/gtkfmrgunc.html

[R36] 并发执行多个任务
来源：http://hz.yuanzhike.top/gtddtxivzj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.vqdsnc.cn/gtiytgkaan.html

[R37] 把输出赋给变量
来源：http://hz.meibo888.top/gtzurblpco.html

files=$(ls -1)
来源：http://hz.svipenyu.cn/gtbosyejyn.html

[R38] 管道串联
来源：http://hz.zhongyouzk.top/gtnybabaiv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zdqjudy.top/gtypjlitrz.html

[R39] 重定向标准输出与错误
来源：http://hz.bjfxy.top/gtljreksyf.html

cmd > out.log 2>&1
来源：http://hz.birdmap.top/gtkiikybzl.html

[R40] 追加写日志
来源：http://hz.birdmap.top/gthpsjdwwx.html

echo "log" >> out.log
来源：http://hz.sxryk.cn/gtabmiolzb.html

[R41] 丢弃输出
来源：http://hz.shuidangran.top/gtxidfdscf.html

cmd >/dev/null 2>&1
来源：http://hz.gaohongyu789.top/gtkforoqap.html

[R42] 输入重定向
来源：http://hz.zhijiandao.cn/gtfctzudcm.html

wc -l < a.txt
来源：http://hz.daxiang520.top/gtdfzykahh.html

[R43] 按名字查找文件
来源：http://hz.fengsongda.top/gteyeymrck.html

find . -name "*.log" -type f
来源：http://hz.jinghuilouyu.cn/gtyardvqwd.html

[R44] 按修改时间查找
来源：http://hz.nwbrower.top/gtuwoutrjc.html

find . -mtime -7 -type f
来源：http://hz.bjfxy.top/gtaehtyoir.html

[R45] 批量删除
来源：http://hz.snrcjt.cn/gtlxpudzzm.html

find . -name "*.tmp" -delete
来源：http://hz.jlsjyb.cn/gtvzeodrgz.html

[R46] 递归替换文件内容
来源：http://hz.wangshuangyany.cn/gtetpwduke.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.aizwys.cn/gtahgotvcm.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gtkvxwyhnb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinqigufen.top/gtlnfevnbw.html

[R48] awk 取指定列
来源：http://hz.jinqigufen.top/gtuqmkkelg.html

awk '{print $1, $3}' a.txt
来源：http://hz.gzhubu.top/gtyghmdvgc.html

[R49] awk 带条件
来源：http://hz.xziqi.cn/gtgxhuukwg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.fzhhl.top/gtylwtbcux.html

[R50] awk 求和
来源：http://hz.aibaodan.cn/gtvwkaauty.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.havefunace.top/gtylbogurn.html

[R51] 排序去重取前几
来源：http://hz.zhaomingkeji.xyz/gtvkdmykem.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cheryme.top/gtxngcedbj.html

[R52] 统计行数
来源：http://hz.hfpthk.cn/gtdxdfxbas.html

wc -l a.txt
来源：http://hz.xinyue.icu/gtfhvujqdy.html

[R53] 查看文件头与实时尾
来源：http://hz.tanke756.top/gtkcxheeuz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ybcxt.top/gtnkobxnfc.html

[R54] 比较两个文件
来源：http://hz.pengpengdd.cyou/gtbgplzxhk.html

diff a.txt b.txt
来源：http://hz.jinqigufen.top/gtjxghfaba.html

[R55] 压缩与解压
来源：http://hz.kuanghao11.cn/gtjlfndxeq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.snrcjt.cn/gtyatyhgcx.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangtech.top/gttvhrnnrk.html

scp file user@host:/path/
来源：http://hz.jlsjyb.cn/gtfnlilnuv.html

[R57] 远程执行命令
来源：http://hz.jiagoushi.top/gtwdjmyzcr.html

ssh user@host 'uptime'
来源：http://hz.yanxiufei.cn/gtlstkmfyz.html

[R58] 下载文件
来源：http://hz.tian-w.cn/gtxalnxyvj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zycfv.cn/gtwbyxwphe.html

[R59] 发 POST JSON
来源：http://hz.gogol.net.cn/gtrraxbsli.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xylfe.cn/gtcaabblln.html

[R60] 只看 HTTP 状态码
来源：http://hz.kuanghao11.cn/gtajrqdwru.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.aizwys.cn/gtcswriibh.html

[R61] 磁盘占用
来源：http://hz.yvedp.cn/gtbfhpuylx.html

df -h;  du -sh *
来源：http://hz.0kj1m.cn/gtbxulxbao.html

[R62] 找最占空间的文件
来源：http://hz.ybcxt.top/gtrkzyubrh.html

du -ah . | sort -rh | head -10
来源：http://hz.sufxvd.cn/gtjyvlxyip.html

[R63] 内存与进程
来源：http://hz.xylfe.cn/gtwulqcqfp.html

free -h;  ps aux | grep nginx
来源：http://hz.yuxming.cn/gtxdtrwckf.html

[R64] 结束进程
来源：http://hz.yuanzhike.top/gtswenuvbz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.aizwys.cn/gthjhabmfw.html

[R65] 查看端口占用
来源：http://hz.hnqzz.top/gtvpjrumqq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yonumen.top/gtwdblpfgx.html

[R66] 定时任务
来源：http://hz.ywan-chungtsiang.top/gtpywjgyzc.html

crontab -e;  crontab -l
来源：http://hz.xuanzx.com/gtmvtjdkpb.html

[R67] 生成随机十六进制串
来源：http://hz.meibo888.top/gtvqdlaxbz.html

openssl rand -hex 16
来源：http://hz.ybcxt.top/gtedwnxthp.html

[R68] 计算文件校验值
来源：http://hz.svipenyu.cn/gtftyrmryh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ywan-chungtsiang.top/gtfvvjheph.html

[R69] 生成随机密码
来源：http://hz.aizwys.cn/gtnssmxvkn.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj20258888.top/gtgtyisfzx.html

[R70] 时间戳与互转
来源：http://hz.xinyue.icu/gtxyghuosm.html

date +%s;  date -d @1700000000
来源：http://hz.cdnleiting.top/gtlmqkslwc.html

[R71] 日期格式化
来源：http://hz.chenlongwang.top/gthdjvgmwu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydzc1.top/gtgiaxuzok.html

[R72] 等待端口就绪
来源：http://hz.birdmap.top/gttzpvwbpo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtluqizlpe.html

[R73] 分割大日志
来源：http://hz.yj20258888.top/gtpvgnghjh.html

split -l 1000 big.log part_
来源：http://hz.316326.xyz/gtwdfmydts.html

[R74] 批量重命名
来源：http://hz.bjfxy.top/gtnycsytmo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.haohaochexian.top/gtnmmomihf.html

[R75] 导出环境变量
来源：http://hz.xingfuxueyuan.xyz/gtiabmtnxg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.0kj1m.cn/gtzzhvnxbj.html

[R76] 使用临时文件
来源：http://hz.yangfankeji.com/gtjxlgivkl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtkmlpoqin.html

[R77] 读取用户输入
来源：http://hz.feifeiyinyue.top/gtuhwsfdqf.html

read -rp "请输入: " ans
来源：http://hz.cucudq.cn/gtbfshryiv.html

[R78] 交互式菜单
来源：http://hz.tianlin.xyz/gtqwgefwfj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.iojbl.cn/gtgkzntfeh.html

[R79] 解析命令行选项
来源：http://hz.chenzaomai.com/gttexnmpew.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.kuanghao11.cn/gtalohquap.html

[R80] 查看脚本执行耗时
来源：http://hz.xuetiantiany.cn/gtpzpfiilx.html

time ./run.sh
来源：http://hz.yj20258.top/gtmhzmhcsb.html

================================================================================
来源：http://hz.jqgufenzy.top/gtiyfmyaus.html

S. C / C++ 专题
来源：http://hz.bjfxy.top/gtgqugkqgy.html

================================================================================
来源：http://hz.ehwqpu.com/gtmsxgvdxc.html

[S01] C：Hello World
来源：http://hz.ybcxt.top/gtxjfvlfnx.html

#include <stdio.h>
来源：http://hz.wangshuangyany.cn/gtcwzlbaqz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yuxming.cn/gtzuktxgjp.html

[S02] C：变量与格式化输出
来源：http://hz.hnxiangtu.top/gtysylllvw.html

int a = 10; printf("%d\n", a);
来源：http://hz.jiagoushi.top/gtfrjvnify.html

[S03] C：读入整数
来源：http://hz.ywan-chungtsiang.top/gtupfzfcqh.html

int x; scanf("%d", &x);
来源：http://hz.jinyuanbaomall.cn/gtnlhggxzm.html

[S04] C：字符串复制
来源：http://hz.redwolf501.top/gtadjhtpva.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.smart0.xyz/gteiygpzdl.html

[S05] C：字符串长度
来源：http://hz.vqdsnc.cn/gtpmdpjulr.html

strlen(s)
来源：http://hz.xuetiantiany.cn/gtygytuzfu.html

[S06] C：字符串比较
来源：http://hz.chenzaomai.com/gtujlyltgh.html

strcmp(a, b) == 0
来源：http://hz.shangyingyoupin.top/gttgcvbhjx.html

[S07] C：数组遍历求和
来源：http://hz.fzhhl.top/gtqezlfeax.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhijiandao.cn/gtopksekbq.html

[S08] C：动态内存分配与释放
来源：http://hz.yueranfly.top/gtcsdqutev.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.vqdsnc.cn/gtwryjigdo.html

[S09] C：结构体定义与初始化
来源：http://hz.birdmap.top/gtmrzleqfw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ehwqpu.com/gtxqfqcpwt.html

[S10] C：指针与解引用
来源：http://hz.svipenyu.cn/gtofoliftu.html

int *p = &a;  *p = 5;
来源：http://hz.hongshengwenyu.top/gttsaeqqfp.html

[S11] C：逐行读文件
来源：http://hz.hongshengwenyu.top/gtcrttxiwt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.daria6918.cn/gtnoxugadz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cheryme.top/gtnleztgbg.html

fclose(f);
来源：http://hz.bjfxy.top/gtfoefmxao.html

[S12] C：写文件
来源：http://hz.iojbl.cn/gtloiirehd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pycfn.com/gtboabokiw.html

[S13] C：宏定义
来源：http://hz.jyoumei.cn/gtqfztcbwf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.iojbl.cn/gtemahoaaz.html

[S14] C：枚举
来源：http://hz.vqdsnc.cn/gtijejjebb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhiwuduotai.top/gtupcwxlzu.html

[S15] C：类型转换
来源：http://hz.gaohongyu789.top/gtrtnnrvze.html

(double) a / b
来源：http://hz.zhixingplan.top/gtmrqjtwpt.html

[S16] C：位操作置位
来源：http://hz.hammf.cn/gtypoaskwe.html

x |= (1 << 3);
来源：http://hz.ivvv.top/gthlqvelvj.html

[S17] C：安全拼接字符串
来源：http://hz.xylfe.cn/gtbwudtgfz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.birdmap.top/gtkcwsgomi.html

[S18] C：命令行参数
来源：http://hz.dashuyun.cn/gtcwlvejcq.html

int main(int argc, char **argv)
来源：http://hz.fzhhl.top/gteawmrfng.html

[S19] C：快速排序
来源：http://hz.dashuyun.cn/gtpgqlfeas.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ehwqpu.com/gtasrbrxeg.html

[S20] C：二分查找
来源：http://hz.yj20258888.top/gtckxjqlvn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj20258.top/gtklqerqzv.html

[S21] C：字符类别判断
来源：http://hz.yvedp.cn/gtnateqwwc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daxiang520.top/gtagsfebzj.html

[S22] C：字符串转数字
来源：http://hz.dianchejie.cn/gtanucbfeo.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.chenzaomai.com/gtwutpurxp.html

[S23] C：随机数
来源：http://hz.nanxuanxn.top/gtihdroioy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhijiandao.cn/gtubpsyhqj.html

[S24] C：获取本地时间
来源：http://hz.guowangkeji.top/gtmaopewfb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.iojbl.cn/gtrmkgylxv.html

[S25] C：内存拷贝
来源：http://hz.nanxinkj.top/gtyvavhvyp.html

memcpy(dst, src, n);
来源：http://hz.c1oappe.top/gtwwstpgez.html

[S26] C：内存清零
来源：http://hz.hfpthk.cn/gtqkprgcav.html

memset(a, 0, sizeof a);
来源：http://hz.cucudq.cn/gthmlolzol.html

[S27] C：定义常量
来源：http://hz.guowangkeji.top/gtaploidgl.html

const double PI = 3.14159;
来源：http://hz.aizwys.cn/gttfhnmxxf.html

[S28] C：静态变量
来源：http://hz.ywan-chungtsiang.top/gthkgfvpqh.html

static int counter = 0;
来源：http://hz.316326.xyz/gtontkxvzl.html

[S29] C：变参函数
来源：http://hz.andypj.xyz/gtpbftyvgc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jlsjyb.cn/gtffrpgntr.html

[S30] C：头文件保护
来源：http://hz.zdqjudy.top/gtuyavgfns.html

#ifndef X_H
来源：http://hz.guannengcc.top/gtlqbtfrqq.html

#define X_H
来源：http://hz.nanxinkj.top/gtaqriifzy.html

#endif
来源：http://hz.ehwqpu.com/gttjswoevq.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtjmwvhhvf.html


<!-- 参考信息 -->