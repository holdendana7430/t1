代发 wailian999

ROLLBACK TO sp1;
来源：http://hz.xuetiantiany.cn/gtxnhzxndw.html

[Q69] 查看执行计划
来源：http://hz.hammf.cn/gtevkrvgrc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.pengpengdd.cyou/gtxpyvimnj.html

[Q70] 更新统计信息
来源：http://hz.redwolf501.top/gtqlbyjfwm.html

ANALYZE TABLE users;
来源：http://hz.316326.xyz/gtrovjjhdr.html

[Q71] 查看建表语句
来源：http://hz.meibo888.top/gtzjmkugot.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.bjfxy.top/gtbjangwdi.html

[Q72] 查看索引
来源：http://hz.meibo888.top/gtaatykphz.html

SHOW INDEX FROM users;
来源：http://hz.xylfe.cn/gttfmfcgej.html

[Q73] 查看表状态
来源：http://hz.zhiwuduotai.top/gtkchijson.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj202588.top/gturwjisnv.html

[Q74] 强制使用索引
来源：http://hz.yonumen.top/gtnlddlarb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuetiantiany.cn/gtpdgwfpfs.html

[Q75] 日期格式化
来源：http://hz.quarkkingdee.top/gtqeagmmnh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.snrcjt.cn/gtgbkxejyb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dashuyun.cn/gtuwopkblm.html

[Q76] 按天统计
来源：http://hz.xylfe.cn/gtpltuiwec.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ivvv.top/gtnywjynnd.html

[Q77] 时间加减
来源：http://hz.ydzc1.top/gtpgggfsff.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxuanxn.top/gtemcanjun.html

[Q78] 当前时间
来源：http://hz.bjfxy.top/gtoqvnvfpd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xinyue.icu/gtzpnpqswv.html

[Q79] 字符串拼接
来源：http://hz.cheryme.top/gtvvhxudbd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinyuanbaomall.cn/gtaxqqdzip.html

[Q80] 字符串截取
来源：http://hz.snrcjt.cn/gtugvfsodd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jlsjyb.cn/gthawcxmvn.html

[Q81] 字符串替换
来源：http://hz.yvedp.cn/gttkxnrhml.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hfpthk.cn/gtocggimwq.html

[Q82] 字符长度与字节长度
来源：http://hz.yj202588.top/gtmwgwoagp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zycfv.cn/gtpubnqltp.html

[Q83] 大小写转换
来源：http://hz.yj20258888.top/gtmhpzjpkh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.iojbl.cn/gtsmhdtldh.html

[Q84] 去除首尾空格
来源：http://hz.yongpay.top/gtqsniqbnv.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtmhbavyxp.html

[Q85] 数值取整
来源：http://hz.yj202588.top/gtuzwhoeki.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinghuilouyu.cn/gthyquuqfz.html

[Q86] 读取 JSON 字段
来源：http://hz.52xcode.cn/gtxuiuryai.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cucudq.cn/gtqhnsefya.html

[Q87] JSON 字段做条件
来源：http://hz.daria6918.cn/gtchurrxqv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.havefunace.top/gtwvjtmneo.html

[Q88] 行转列（条件聚合）
来源：http://hz.smart0.xyz/gtbqxsjywa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tianlin.xyz/gtbrojtumu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cheryme.top/gtllhelenq.html

[Q89] 判断表是否存在
来源：http://hz.gzhubu.top/gtbpeyqmvb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tianlin.xyz/gtiuklufrx.html

[Q90] 生成序号列
来源：http://hz.zhijiandao.cn/gtrfylyczn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydjk.org.cn/gtculoemax.html

================================================================================
来源：http://hz.9152youxi.cn/gtugccqdnq.html

R. Bash 专题
来源：http://hz.yj20258888.top/gtoxxydhrk.html

================================================================================
来源：http://hz.daria6918.cn/gtadqtowhj.html

[R01] shebang 与严格模式
来源：http://hz.cheryme.top/gtoxytnygi.html

#!/usr/bin/env bash
来源：http://hz.zhengqikj.top/gtkprbuoxj.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gtwthkuazq.html

[R02] 变量赋值与使用
来源：http://hz.yj20258888.top/gtrybomdaq.html

name="Tom"; echo "$name"
来源：http://hz.zycfv.cn/gtpnczablo.html

[R03] 只读变量
来源：http://hz.ppjwa.cn/gtdbbqfigv.html

readonly PI=3.14
来源：http://hz.gogol.net.cn/gtvpcergig.html

[R04] 位置参数
来源：http://hz.chenjidiqi.icu/gteyzxznrh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zdqjudy.top/gtxzbicjet.html

[R05] 参数默认值
来源：http://hz.fzhhl.top/gtjdsuglqz.html

name="${1:-default}"
来源：http://hz.ybcxt.top/gthndwzseq.html

[R06] 判断命令是否存在
来源：http://hz.mhx1999.top/gtkcfhzekn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.pycfn.com/gtbullkrkm.html

[R07] if 判断文件
来源：http://hz.xinyue.icu/gtbuxcxgrd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtjbasiuvf.html

[R08] 数值比较
来源：http://hz.havefunace.top/gtkdthiolg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.snrcjt.cn/gtinrmctvw.html

[R09] 字符串比较
来源：http://hz.shzxlz.cn/gttqjayogu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shangyingyoupin.top/gtbyfhhxle.html

[R10] 正则匹配
来源：http://hz.hongshengwenyu.top/gtbcozdfrk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nwbrower.top/gtgienwoph.html

[R11] case 多分支
来源：http://hz.wangshuangyany.cn/gtimlfqzuf.html

case "$1" in
来源：http://hz.aibaodan.cn/gtqttuogoo.html

start) echo "启动" ;;
来源：http://hz.fzhhl.top/gtssmcyxvk.html

stop)  echo "停止" ;;
来源：http://hz.yanxiufei.cn/gtoevsqjqr.html

*)     echo "未知命令" ;;
来源：http://hz.xuetiantiany.cn/gttbrlpcxi.html

esac
来源：http://hz.shangyingyoupin.top/gthnyisrov.html

[R12] for 遍历文件
来源：http://hz.zhijiandao.cn/gtwjrrpeyv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cqqwz.cn/gtzxqmwxkx.html

[R13] for 计数循环
来源：http://hz.ppjwa.cn/gtubuhcgrn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.andypj.xyz/gtjbqiflyl.html

[R14] C 风格 for
来源：http://hz.andypj.xyz/gtzmjilsqs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenzaomai.com/gtkwxddrzi.html

[R15] while 逐行读文件
来源：http://hz.jianghu66.top/gtadrjvfix.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xylfe.cn/gtqsxuyyrs.html

[R16] until 等待条件
来源：http://hz.quarkkingdee.top/gtcniusuer.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hongshengwenyu.top/gtdhbijcwi.html

[R17] 数组定义与取值
来源：http://hz.xylfe.cn/gtxfzwkpzp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jlsjyb.cn/gtourcbnnl.html

[R18] 遍历数组
来源：http://hz.sxryk.cn/gtjxcdqgzb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhengqikj.top/gtvoisuvlw.html

[R19] 数组长度
来源：http://hz.shzxlz.cn/gtfceubebw.html

echo "${#arr[@]}"
来源：http://hz.hysaishi.cn/gtqgstiiyx.html

[R20] 关联数组（字典）
来源：http://hz.tianlin.xyz/gtervgwxfv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhengqikj.top/gtjccxcugw.html

[R21] 字符串长度
来源：http://hz.cheryme.top/gtzikrtfur.html

echo "${#s}"
来源：http://hz.hnqzz.top/gtyywxhwmc.html

[R22] 截取子串
来源：http://hz.jiagoushi.top/gtcvcgajrl.html

echo "${s:0:5}"
来源：http://hz.0kj1m.cn/gtqmtenvle.html

[R23] 字符串替换
来源：http://hz.ydzc1.top/gtajjqxfxq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.snrcjt.cn/gtyqwrjpfz.html

[R24] 大小写转换
来源：http://hz.fengsongda.top/gtzwhbujyl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nanxinkj.top/gtlthearqh.html

[R25] 去后缀 / 去前缀
来源：http://hz.xylfe.cn/gttkbocgwf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cdnleiting.top/gtuxkhinpr.html

[R26] 命令替换
来源：http://hz.9152youxi.cn/gtoldcqrpv.html

now=$(date +%F); echo "$now"
来源：http://hz.tian-w.cn/gtwpzuchpd.html

[R27] 算术展开
来源：http://hz.tanke756.top/gtsthrodvw.html

echo $((1 + 2 * 3))
来源：http://hz.ydjk.org.cn/gtsxealmmx.html

[R28] 浮点运算
来源：http://hz.9152youxi.cn/gtahvwklja.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj202588.top/gtftcyvqbd.html

[R29] 定义函数
来源：http://hz.sweek.top/gteghagssx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhengqikj.top/gtgrokbwbs.html

[R30] 函数返回状态码
来源：http://hz.xuanzx.com/gtryvxftad.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sweek.top/gtcgoyszaw.html

[R31] 局部变量
来源：http://hz.wangdashe.top/gtdvqwtkqw.html

f() { local x=1; echo "$x"; }
来源：http://hz.cucudq.cn/gtqvsyzgrk.html

[R32] 参数个数校验
来源：http://hz.hnxiangtu.top/gtetrluwok.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ydjk.org.cn/gtnwbrmufs.html

[R33] 捕获错误并提示行号
来源：http://hz.jqgufenzy.top/gtmqovakoj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenzaomai.com/gthlxxgujn.html

[R34] 退出时清理
来源：http://hz.hywenlv.cn/gtmibxcibh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.mhx1999.top/gtllywxjcm.html

[R35] 后台执行并等待
来源：http://hz.jyoumei.cn/gtrcfpoawl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ywan-chungtsiang.top/gtartaerfp.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangtech.top/gtvrvaaokl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hongshengwenyu.top/gtjegjkheq.html

[R37] 把输出赋给变量
来源：http://hz.quarkkingdee.top/gtrplptltt.html

files=$(ls -1)
来源：http://hz.ybcxt.top/gtccycyovm.html

[R38] 管道串联
来源：http://hz.yj20258.top/gtwfxxouom.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgfzy.top/gtltpqdped.html

[R39] 重定向标准输出与错误
来源：http://hz.daria6918.cn/gthmcondhm.html

cmd > out.log 2>&1
来源：http://hz.yuanzhike.top/gttqpzzxet.html

[R40] 追加写日志
来源：http://hz.cqqwz.cn/gturujfmvj.html

echo "log" >> out.log
来源：http://hz.tanke756.top/gtvfubloqm.html

[R41] 丢弃输出
来源：http://hz.aizwys.cn/gtbdbpxfee.html

cmd >/dev/null 2>&1
来源：http://hz.mhx1999.top/gttfsbntwp.html

[R42] 输入重定向
来源：http://hz.jianghu66.top/gtvajbxsil.html

wc -l < a.txt
来源：http://hz.fzhhl.top/gtrkbzqiyz.html

[R43] 按名字查找文件
来源：http://hz.yj202588.top/gtsihqumen.html

find . -name "*.log" -type f
来源：http://hz.yongpay.top/gtlsryqunv.html

[R44] 按修改时间查找
来源：http://hz.nwbrower.top/gthekgzjag.html

find . -mtime -7 -type f
来源：http://hz.kuanghao11.cn/gtmqoauauw.html

[R45] 批量删除
来源：http://hz.shuidangran.top/gtsjiaszrg.html

find . -name "*.tmp" -delete
来源：http://hz.ivvv.top/gtnkejhbml.html

[R46] 递归替换文件内容
来源：http://hz.gzhubu.top/gtflwfcoim.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.andypj.xyz/gtftjsedil.html

[R47] sed 单行替换
来源：http://hz.jinqigufen.top/gtrzagtldm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenzaomai.com/gttscukqra.html

[R48] awk 取指定列
来源：http://hz.sweek.top/gtjowjwllm.html

awk '{print $1, $3}' a.txt
来源：http://hz.mhx1999.top/gttdmysyhf.html

[R49] awk 带条件
来源：http://hz.dianchejie.cn/gtpecqrueb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ywan-chungtsiang.top/gtkdflohbl.html

[R50] awk 求和
来源：http://hz.jianghu66.top/gtcmgvfxwo.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnxiangtu.top/gttwmmgcqw.html

[R51] 排序去重取前几
来源：http://hz.meibo888.top/gtirpmpavs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tianlin.xyz/gtsteytnge.html

[R52] 统计行数
来源：http://hz.gzhubu.top/gtpdnrfswg.html

wc -l a.txt
来源：http://hz.chenzaomai.com/gtfscaxszz.html

[R53] 查看文件头与实时尾
来源：http://hz.zhijiandao.cn/gtfyeptadg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.pengpengdd.cyou/gtcgivavmr.html

[R54] 比较两个文件
来源：http://hz.yongpay.top/gtxstkybri.html

diff a.txt b.txt
来源：http://hz.birdmap.top/gtwqnoapfj.html

[R55] 压缩与解压
来源：http://hz.fzhhl.top/gtdoxrmcyb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zycfv.cn/gtmdyfsspq.html

[R56] 远程拷贝
来源：http://hz.chenjidiqi.icu/gtksouygnf.html

scp file user@host:/path/
来源：http://hz.zycfv.cn/gthvjsuian.html

[R57] 远程执行命令
来源：http://hz.vqdsnc.cn/gtzipvhocb.html

ssh user@host 'uptime'
来源：http://hz.52xcode.cn/gtisovfshi.html

[R58] 下载文件
来源：http://hz.yanxiufei.cn/gtaskjzywl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.c1oappe.top/gtyawvvpen.html

[R59] 发 POST JSON
来源：http://hz.xuetiantiany.cn/gtjdszaruc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ybcxt.top/gtpxzfihfq.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtpyialdzx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xinyue.icu/gtjmwdblhm.html

[R61] 磁盘占用
来源：http://hz.sufxvd.cn/gtmbxihnhj.html

df -h;  du -sh *
来源：http://hz.zhoulong.xyz/gttmvwfyks.html

[R62] 找最占空间的文件
来源：http://hz.zhiwuduotai.top/gthcnmwcbj.html

du -ah . | sort -rh | head -10
来源：http://hz.c1oappe.top/gtojupghje.html

[R63] 内存与进程
来源：http://hz.svipenyu.cn/gtarunzbib.html

free -h;  ps aux | grep nginx
来源：http://hz.hongshengwenyu.top/gtxxtdoept.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtbgeizfom.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shzxlz.cn/gtjrevpoaq.html

[R65] 查看端口占用
来源：http://hz.birdmap.top/gtilhgjjvz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinqigufen.top/gtqmgywgam.html

[R66] 定时任务
来源：http://hz.tian-w.cn/gtsbpriolk.html

crontab -e;  crontab -l
来源：http://hz.yangfankeji.com/gtbprbndep.html

[R67] 生成随机十六进制串
来源：http://hz.shanyushiyangkeji.top/gtrvgjouyx.html

openssl rand -hex 16
来源：http://hz.xziqi.cn/gttdcpnfic.html

[R68] 计算文件校验值
来源：http://hz.zhoulong.xyz/gtahnrtxbm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dianchejie.cn/gtlktkdmpe.html

[R69] 生成随机密码
来源：http://hz.zdqjudy.top/gtxkqudmcv.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gttimybaxo.html

[R70] 时间戳与互转
来源：http://hz.zycfv.cn/gtvmblysjm.html

date +%s;  date -d @1700000000
来源：http://hz.gaohongyu789.top/gtyceotnnp.html

[R71] 日期格式化
来源：http://hz.shangyingyoupin.top/gtixfmmnby.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jqgfzy.top/gtnfwyewrs.html

[R72] 等待端口就绪
来源：http://hz.zycfv.cn/gtcccxellc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ywan-chungtsiang.top/gtncirmkym.html

[R73] 分割大日志
来源：http://hz.ppjwa.cn/gtzysqafpd.html

split -l 1000 big.log part_
来源：http://hz.snrcjt.cn/gtdssapwvs.html

[R74] 批量重命名
来源：http://hz.ivvv.top/gtjnhxwjvm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhaomingkeji.xyz/gtxhufzuhu.html

[R75] 导出环境变量
来源：http://hz.snrcjt.cn/gtrzbtvvlf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.52xcode.cn/gtvyxgwndh.html

[R76] 使用临时文件
来源：http://hz.pycfn.com/gtgjibsvdb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangkeji.top/gtktzhoxjv.html

[R77] 读取用户输入
来源：http://hz.xingfuxueyuan.xyz/gtclfoxbcy.html

read -rp "请输入: " ans
来源：http://hz.pycfn.com/gtddokwdgc.html

[R78] 交互式菜单
来源：http://hz.hammf.cn/gtmkotegwj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shangyingyoupin.top/gtwxosgihx.html

[R79] 解析命令行选项
来源：http://hz.cucudq.cn/gthkumuleb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hywenlv.cn/gtnfuftyte.html

[R80] 查看脚本执行耗时
来源：http://hz.jinghuilouyu.cn/gtaipxnbsz.html

time ./run.sh
来源：http://hz.hfpthk.cn/gtdrudvlar.html

================================================================================
来源：http://hz.jiagoushi.top/gtughavfes.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtllmoesxv.html

================================================================================
来源：http://hz.hnqzz.top/gtuneqwhsq.html

[S01] C：Hello World
来源：http://hz.cashguo.top/gtqrdyvqbu.html

#include <stdio.h>
来源：http://hz.52xcode.cn/gtconjqdcb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.dianchejie.cn/gtdjsbsjwo.html

[S02] C：变量与格式化输出
来源：http://hz.mhx1999.top/gtjjdixxny.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinghuilouyu.cn/gtajflndzl.html

[S03] C：读入整数
来源：http://hz.birdmap.top/gtdvkbhgqo.html

int x; scanf("%d", &x);
来源：http://hz.52xcode.cn/gtxlelqbkl.html

[S04] C：字符串复制
来源：http://hz.zhixingplan.top/gtickqezbj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cheryme.top/gtveivzayn.html

[S05] C：字符串长度
来源：http://hz.aizwys.cn/gtszsvezio.html

strlen(s)
来源：http://hz.bjfxy.top/gtykrswctc.html

[S06] C：字符串比较
来源：http://hz.andypj.xyz/gtwkcohvme.html

strcmp(a, b) == 0
来源：http://hz.aibaodan.cn/gtsuhwhwxa.html

[S07] C：数组遍历求和
来源：http://hz.jiagoushi.top/gtyqyawvzq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hysaishi.cn/gtucussfxx.html

[S08] C：动态内存分配与释放
来源：http://hz.jinqigufen.top/gtdfieimsu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhoulong.xyz/gtoutcuupc.html

[S09] C：结构体定义与初始化
来源：http://hz.vqdsnc.cn/gtuemjuupy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gzhubu.top/gthggssgpd.html

[S10] C：指针与解引用
来源：http://hz.pycfn.com/gtyyplicgt.html

int *p = &a;  *p = 5;
来源：http://hz.gzhubu.top/gtmnagghtp.html

[S11] C：逐行读文件
来源：http://hz.cqqwz.cn/gtfruhbjmz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.316326.xyz/gtkbffkasj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxuanxn.top/gtrhsekxcs.html

fclose(f);
来源：http://hz.aizwys.cn/gtpkefecwy.html

[S12] C：写文件
来源：http://hz.zhaomingkeji.xyz/gthwlyzbgn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ppjwa.cn/gtihgfnwaf.html

[S13] C：宏定义
来源：http://hz.bjfxy.top/gtoruwkjsj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.birdmap.top/gtrqvytnma.html

[S14] C：枚举
来源：http://hz.xziqi.cn/gtvtxpeseg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xingfuxueyuan.xyz/gtzqhmzaks.html

[S15] C：类型转换
来源：http://hz.gotoacloud.top/gttaeapbvk.html

(double) a / b
来源：http://hz.xuanzx.com/gtefrssjtz.html

[S16] C：位操作置位
来源：http://hz.yvedp.cn/gteqkgmrtz.html

x |= (1 << 3);
来源：http://hz.yj20258.top/gtxyzlbvrx.html

[S17] C：安全拼接字符串
来源：http://hz.svipenyu.cn/gtisuuemaf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nwbrower.top/gtolqftwpw.html

[S18] C：命令行参数
来源：http://hz.yj20258888.top/gtvfzatttx.html

int main(int argc, char **argv)
来源：http://hz.chenzaomai.com/gtjdkymlwt.html

[S19] C：快速排序
来源：http://hz.shanyushiyangkeji.top/gtodvdsrtp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtozudypzw.html

[S20] C：二分查找
来源：http://hz.cheryme.top/gtffdzaakk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtekjjvmra.html

[S21] C：字符类别判断
来源：http://hz.jqgufenzy.top/gtcaumoumt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sufxvd.cn/gtclqytoxl.html

[S22] C：字符串转数字
来源：http://hz.yongpay.top/gtktwutsyl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.c1oappe.top/gtrgubpbij.html

[S23] C：随机数
来源：http://hz.0kj1m.cn/gtjzcwlsrw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.havefunace.top/gtdioximqh.html

[S24] C：获取本地时间
来源：http://hz.andypj.xyz/gttbfkdztu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jianghu66.top/gtqbjxebja.html

[S25] C：内存拷贝
来源：http://hz.jyoumei.cn/gtyznxmrfs.html

memcpy(dst, src, n);
来源：http://hz.jyoumei.cn/gtqxvpgyhg.html

[S26] C：内存清零
来源：http://hz.ivvv.top/gtmlopwrio.html

memset(a, 0, sizeof a);
来源：http://hz.xylfe.cn/gthdbqmtts.html

[S27] C：定义常量
来源：http://hz.shangyingyoupin.top/gtdbsqxqdj.html

const double PI = 3.14159;
来源：http://hz.pycfn.com/gtrvslthps.html

[S28] C：静态变量
来源：http://hz.0kj1m.cn/gtudntiaaw.html

static int counter = 0;
来源：http://hz.iojbl.cn/gtxxxmjmto.html

[S29] C：变参函数
来源：http://hz.gzhubu.top/gtyqkqzqit.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.havefunace.top/gtoqewrueb.html

[S30] C：头文件保护
来源：http://hz.tanke756.top/gtqperjzng.html

#ifndef X_H
来源：http://hz.chenzaomai.com/gtvotwlleo.html

#define X_H
来源：http://hz.yueranfly.top/gtajmccfij.html

#endif
来源：http://hz.xuetiantiany.cn/gtviibyiql.html

[S31] C++：Hello World
来源：http://hz.9152youxi.cn/gtjvegvxfy.html

#include <iostream>
来源：http://hz.ywan-chungtsiang.top/gtjvlklrcs.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.52xcode.cn/gtparlnyly.html

[S32] C++：字符串
来源：http://hz.meibo888.top/gtalfoaacd.html

std::string s = "hi";  s += "!";
来源：http://hz.guannengcc.top/gtcyjljtya.html

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gtviololsh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.fengsongda.top/gtomvrnstx.html

[S34] C++：遍历 vector
来源：http://hz.yongpay.top/gtdvgaljlh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gaohongyu789.top/gtzcdycbfq.html

[S35] C++：map
来源：http://hz.yj20258.top/gtnplsunhy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtplwpxknc.html

[S36] C++：unordered_map
来源：http://hz.316326.xyz/gtjyaupkdr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gtqwpgfpnn.html

[S37] C++：set
来源：http://hz.hysaishi.cn/gtfhozxixf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fengsongda.top/gtrldkpvqy.html

[S38] C++：排序
来源：http://hz.ivvv.top/gtnuxmryqv.html

std::sort(v.begin(), v.end());
来源：http://hz.guannengcc.top/gtjxpiapzv.html


<!-- 参考信息 -->